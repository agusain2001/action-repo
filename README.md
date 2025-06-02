# GitHub Action Repository

This repository is part of the GitHub Webhook Monitor system. It serves as the repository that will send webhook events to the webhook receiver.

## Setup

1. Configure this repository to send webhook events to your webhook receiver endpoint:
   - Go to repository Settings > Webhooks
   - Add webhook
   - Set Payload URL to your webhook receiver endpoint (e.g., https://your-webhook-receiver.com/api/webhook)
   - Set Content type to `application/json`
   - Select events: Push, Pull requests
   - Enable the webhook

## Testing

After configuration, you can test the webhook integration by:
1. Making a push to this repository
2. Creating a pull request
3. Merging a pull request

These actions will trigger webhook events that will be sent to your webhook receiver.

## Related Repository

This repository works in conjunction with the webhook-repo, which contains the webhook receiver and UI.
