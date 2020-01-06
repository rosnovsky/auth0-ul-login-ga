# Add Google Analytics to Universal Login pages

In your management dashboard, go to Universal Login, then select Classic or New experience, and tab over to "Login" section right above.

Then follow this guide: https://auth0.com/docs/analytics/guides/google-analytics

You'll end up with something like this:

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
  <title>Sign In with Auth0</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <script>
      window.auth0AnalyticsOptions = {
        'google-analytics': {
            id: 'UA-XXXXXXXXX-X',
            preloaded: true
        }
      }
    </script>
  <script src="https://cdn.auth0.com/js/lock/11.20/lock.min.js"></script>
  <script src="https://cdn.auth0.com/js/analytics/1.3.1/analytics.min.js"></script>
</head>
<body>
<!-- THE REST OF THE PAGE ->
...
```
