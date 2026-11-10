# CICT Org Fair

**Live Website:** https://mikhael-gedorio.github.io/GEDORIO-ASSIGNMENT_7/

A Flutter-based mobile and web application for the West Visayas State University College of Information and Communications Technology (CICT) Organization Fair.

## Features

- Browse organization fair events.
- View event details, schedules, venues, and descriptions.
- View event cancellation status.
- Retrieve event information from a hosted Strapi CMS.
- View application version and build number.

## Technologies Used

- Flutter and Dart
- Strapi CMS
- PostgreSQL
- GitHub Actions
- GitHub Pages

## CMS Configuration

The application connects to a hosted Strapi CMS using the following configuration:

- CMS: Strapi
- CMS URL: https://strapi-org-fair.onrender.com

Public read permissions are enabled for the Fair Events collection. No private API token is included in the Flutter application.

## Running Locally

1. Install Flutter.
2. Clone this repository.
3. Run `flutter pub get`.
4. Configure your local `cms.json` file.
5. Run the application:

```bash
flutter run -d chrome --dart-define-from-file=cms.json
```

## Building for Web

```bash
flutter build web --release --dart-define-from-file=cms.json
```

## Deployment

The web application is deployed through GitHub Actions to GitHub Pages whenever changes are pushed to the `main` branch.

## Version

- Version: 1.1.0
- Build number: 2
