# Clarity Hub Connector

<img src="./clarity-hub-approved-logo.png" alt="Clarity Hub" width="140" height="140">

Connect an AI assistant to your authorized Clarity Hub account to work with projects, WhatsApp conversations, tasks and documents.

**Requires an existing approved Clarity Hub account.** Adding the connector does not create a Hub account, enroll a company, or grant additional access. Contact Clarity Construction to request access. Availability in an AI application also depends on that application's plan and organization settings.

## Server address

```text
https://hub.clarity-construction.com/api/mcp
```

Use OAuth sign-in. Do not put an account password, API key, access token or private connector URL into the public server-address field.

## Connect in Claude

1. Open Claude's **Settings → Connectors** and choose to add a custom connector.
2. Name it **Clarity Hub** and enter the server address above.
3. Select **Sign in now** and automatic OAuth client registration if those options are shown.
4. Connect, sign in to your approved Hub account, and review the access requested before authorizing.
5. In a new conversation, ask: “Show my projects and what needs my attention.”

Custom connection and an approved public directory listing are separate. These instructions describe a custom connection.

## Connect in Grok

1. Open [Grok Connectors](https://grok.com/connectors).
2. Choose **New Connector → Custom**, name it **Clarity Hub**, and enter the server address above.
3. Follow the OAuth sign-in flow and review the requested access before authorizing.
4. Ask Grok to list the projects available to your connected account.

Your Grok organization may require an administrator to make custom connectors available first. A custom connection does not establish marketplace approval.

## Connect in ChatGPT

If your organization has made the **Clarity Hub** workspace plugin available, install/connect that entry and sign in with your approved Hub account. Contact your workspace administrator if it is not available.

Public directory publication is a separate review process. This document does not claim a public listing has been approved.

## What the connector can do

Depending on your account's permissions and enabled integrations, it can:

- Find projects and read their stages, records, documents and accessible conversations.
- Summarize recent messages and walkthroughs with references to available source information.
- Show tasks, notifications, deadlines and items needing attention.
- Draft tasks or messages and make supported project updates when requested.
- Send requested WhatsApp messages where your Hub permissions and connected number allow it.

The connector includes tools that can change records, create CRM entries or send messages immediately. Review the proposed project, recipient, assignee, dates and content before requesting an action. Not every write tool creates an approval draft. If you want a draft, say so explicitly; for example, “Draft this message; do not send it.”

## Access and data

OAuth connects the assistant to a Hub account. The server advertises `hub` for access, `hub.write` for supported changes and `offline_access` for refresh access; review the actual consent screen for the access being requested. A connected application can only act within the permissions the Hub grants to that account. Private conversations are not public merely because the connector address is public.

Only connect AI applications you trust. Information requested through a connector is returned to the AI application you are using, which has its own privacy and account settings. Do not give anyone your own login or share a real employee's account for testing.

Read the [Clarity Hub privacy policy](https://hub.clarity-construction.com/privacy). For questions about account access, data handling, deletion or a connected application's access, contact [chris@clarity-construction.com](mailto:chris@clarity-construction.com).

## Disconnect or troubleshoot

- Remove or disconnect Clarity Hub in your AI application's connector settings when you no longer want that connection.
- Use the Hub's Connections settings to review your assistant sign-ins and revoke the relevant connection when needed.
- If new tools are missing after an update, use the application's refresh/reconnect option where available and start a new conversation. Public-directory changes can require additional platform checks.
- An access-denied response should be resolved through your Hub administrator. Do not disable authentication, share another user's credentials, or substitute a secret in the server URL.
- When requesting support, provide the application name, approximate time and error message. Do not email passwords, access tokens or full private chat exports.

## Support

Clarity Construction: [chris@clarity-construction.com](mailto:chris@clarity-construction.com).

This repository contains public connection instructions only. It does not contain the private Hub application source, customer records or credentials.
