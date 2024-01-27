# Google Calendar API Integration with Node.js

This Node.js application demonstrates integration with the Google Calendar API. It allows users to authenticate via Google, list their calendars, and view upcoming events in their Google Calendar.

## Features

- OAuth2 Google Authentication
- Listing all Google Calendars
- Viewing upcoming events in specified Google Calendars

## Getting Started

### Prerequisites

- Node.js installed on your machine
- A Google Cloud Platform account
- A project created in the Google Developers Console with the Google Calendar API enabled
- OAuth 2.0 credentials (Client ID and Client Secret) in your Google project

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/adanzweig/nodejs-google-calendar.git
   ```
2. Navigate to the project directory:
   ```
   cd nodejs-google-calendar
   ```
3. Install the required dependencies:
   ```
   npm install
   ```
4. Create a `.env` file in the root of your project and add your Google OAuth2 credentials:
   ```
   CLIENT_ID=your_client_id
   SECRET_ID=your_client_secret
   REDIRECT=your_redirect_uri
   ```
5. Start the server:
   ```
   npm start
   ```

## Usage

1. Open your browser and navigate to `http://localhost:3000`.
2. You will be redirected to the Google sign-in page.
3. After signing in and granting permissions, you will be redirected back with a message indicating a successful login.
4. Access `http://localhost:3000/calendars` to list all your Google Calendars.
5. Access `http://localhost:3000/events` to list the upcoming events from your primary Google Calendar. You can specify a different calendar by adding `?calendar=your_calendar_id` to the URL.

## Contributing

Contributions are welcome. Please open an issue first to discuss what you would like to change or add.

## License

[MIT](https://choosealicense.com/licenses/mit/)

## Acknowledgements

- [Google APIs Node.js Client](https://github.com/googleapis/google-api-nodejs-client)
- [Google Calendar API Documentation](https://developers.google.com/calendar)
