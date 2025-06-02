# WordPress Flutter CMS

This project uses WordPress as a headless CMS backend and Flutter for the frontend application.

## Setup Instructions

### Backend (WordPress)

1. Start the WordPress server:
   ```bash
   docker-compose up -d
   ```

2. Access WordPress admin at:
   ```
   http://localhost:8080/wp-admin
   ```

3. Install and activate required plugins:
   - WP REST API
   - JWT Authentication for WP REST API
   - Advanced Custom Fields (ACF)
   - ACF to REST API

### Frontend (Flutter)

The Flutter frontend will be implemented in a separate directory. Follow these steps:

1. Create a new Flutter project:
   ```bash
   flutter create frontend
   cd frontend
   flutter run
   ```

2. Configure the WordPress REST API endpoint in your Flutter application.

## Development

- WordPress backend runs on: `http://localhost:8080`
- WordPress REST API available at: `http://localhost:8080/wp-json`
- Flutter frontend will be developed in the `frontend` directory

## Project Structure

```
├── docker-compose.yml    # Docker configuration for WordPress
├── frontend/            # Flutter application (to be created)
└── README.md           # Project documentation
```