# How to Enable Integrations

## Context

We have integrations with the following platforms:

- Airmeet (Virtual Events)
- Airtable (CRM)
- Crunchbase (Company Database)
- Google (Authentication)
- Mailchimp (Email Marketing)
- Postmark (Email)
- Sentry (Error Monitoring)
- Slack (Community Home, Authentication)
- Statsig (Feature Flag)
- SwagUp (Swag Packs)

## Airmeet

To enable the **Airmeet** integration:

1. See Section 3.1 of
   [this](https://help.airmeet.com/support/solutions/articles/82000467794-airmeet-public-api)
   Airmeet documentation to generate an access token/key.
2. In `/api/.env`, set the following variables:

   ```
   AIRMEET_ACCESS_KEY
   AIRMEET_SECRET_KEY
   ```

## Airtable

To enable the **Airtable** integration:

1. See [this](https://support.airtable.com/docs/creating-personal-access-tokens)
   Airtable documentation to generate a personal access token.
2. Create an Airtable base and grab the base ID. You can read
   [this](https://support.airtable.com/docs/finding-airtable-ids) documentation
   for instructions on how to do so.
3. In `/api/.env`, set the following variable:
   ```
   AIRTABLE_API_KEY
   AIRTABLE_EVENT_REGISTRATIONS_BASE_ID
   AIRTABLE_FAMILY_BASE_ID
   ```

## Crunchbase

To enable the **Crunchbase** integration:

1. See [this](https://data.crunchbase.com/docs/crunchbase-basic-getting-started)
   Crunchbase documentation to generate an API key.
2. In `/member-profile/.env`, the following variable:
   ```
   CRUNCHBASE_BASIC_API_KEY
   ```

## Google

To enable the **Google** integration:

1. In the Google Cloud Console, create an OAuth 2.0 Client ID.
   - For the "Authorized JavaScript Origins", you can set:
     - `http://localhost:3000`
     - `http://localhost:3001`
   - For the "Authorized Redirect URIs", you can set:
     - `http://localhost:8080/oauth/google`
2. In `/api/.env`, the following variables:
   ```
   GOOGLE_CLIENT_ID
   GOOGLE_CLIENT_SECRET
   ```
3. In `/admin-dashboard/.env`, the following variables:
   ```
   GOOGLE_CLIENT_ID
   ```
4. In `/member-profile/.env`, the following variables:
   ```
   GOOGLE_CLIENT_ID
   ```

## Mailchimp

To enable the **Mailchimp** integration:

1. See [this](https://mailchimp.com/help/about-api-keys) Mailchimp documentation
   to generate an API key.
2. In `/api/.env`, set the following variables:
   ```
   MAILCHIMP_API_KEY
   MAILCHIMP_AUDIENCE_ID
   MAILCHIMP_SERVER_PREFIX
   ```

## Postmark

To enable the **Postmark** integration:

1. See
   [this](https://postmarkapp.com/support/article/1008-what-are-the-account-and-server-api-tokens)
   Postmark documentation to generate an API key.
2. In `/api/.env`, set the following variable:
   ```
   POSTMARK_API_TOKEN
   ```

## Sentry

To enable the **Sentry** integration:

1. You probably don't need to enable this integration but in case you want to,
   proceed with the following steps.
2. See
   [this](https://docs.sentry.io/product/sentry-basics/concepts/dsn-explainer)
   Sentry documentation on how to get your DSN.
3. In `/api/.env`, set the following variable:
   ```
   SENTRY_DSN
   ```
4. In `/member-profile/.env`, set the following variable:
   ```
   SENTRY_DSN
   ```
5. In `/admin-dashboard/.env`, set the following variable:
   ```
   SENTRY_DSN
   ```

## Slack

To enable the **Slack** integration:

1.
2. In `/api/.env`, set the following variables:
   ```
   SLACK_ANNOUNCEMENTS_CHANNEL_ID
   SLACK_ADMIN_TOKEN
   SLACK_BIRTHDAYS_CHANNEL_ID
   SLACK_BOT_TOKEN
   SLACK_CLIENT_ID
   SLACK_CLIENT_SECRET
   SLACK_INTRODUCTIONS_CHANNEL_ID
   SLACK_SIGNING_SECRET
   ```
3. In `/member-profile/.env`, set the following variables:
   ```
   SLACK_CLIENT_ID
   SLACK_TEAM_ID
   ```

## Statsig

To enable the **Statsig** integration:

1.
2. In `/api/.env`, set the following variables:
   ```
   STATSIG_SECRET_KEY
   ```
3. In `/member-profile/.env`, set the following variables:
   ```
   STATSIG_SECRET_KEY
   ```

## SwagUp

To enable the **SwagUp** integration:

1.
2. In `/api/.env`, set the following variables:
   ```
   SWAG_UP_CLIENT_ID
   SWAG_UP_CLIENT_SECRET
   ```
3. In `/member-profile/.env`, set the following variables:
   ```
   SWAG_UP_CLIENT_ID
   SWAG_UP_CLIENT_SECRET
   ```
