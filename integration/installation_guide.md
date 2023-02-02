Pangea is a collection of security services, all API-based, that can quickly and easily be added to any cloud application, embedded in the runtime code. Pangea provides app builders with a wide selection of security services so they can easily embed security into their application. It’s similar in nature to AWS for Compute APIs, Twilio for Communications APIs, Stripe for Billing APIs. And now there is Pangea for Security APIs.

## Prerequisites

1. An Auth0 account and tenant. [Sign up for free](https://auth0.com/signup).
2. A Pangea account [Sign up for free](https://pangea.cloud/signup?utm_medium=auth0-marketplace&utm_source=marketplace&utm_campaign=auth0-marketplace).

## Set up Pangea

To configure the integration with Pangea:

1. Configure Pangea Secure Audit Log, Embargo, Domain Intel and IP Intel following [the configuration guide](https://pangea.cloud/docs/getting-started/configure-services/).
2. When you create your token in the guide, make sure it also has access to Secure Audit Log, Embargo, Domain Intel and IP Intel 
3. Save your Pangea token and Pangea domain
4. Select your providers for Domain Intel and IP Intel

## Add the Auth0 Action

**Note:** Once the Action is successfully deployed, All assigned flows will be affected by this integration. Before activating the integration in production, [install and verify this Action on a test tenant](https://auth0.com/docs/get-started/auth0-overview/create-tenants/set-up-multiple-environments).

1. Select **Add Integration** (at the top of this page)
1. Read the necessary access requirements, and select **Continue**
1. Configure the integration using the following fields:
   * DOMAIN - The Pangea domain for the organization
   * TOKEN - The token that you saved from the Pangea configuration guide which has access to Secure Audit Log and Domain Intel
   * IP_PROVIDER - The selected provider for IP Intel (e.g. crowdstrike)
   * DOMAIN_PROVIDER - The selected provider for Domain Intel (e.g. domaintools)
1. Add the integration to your Library by selecting **Create**
1. In the modal that appears, select the **Add to flow** link
1. Drag the Action into the desired location in the flow
1. Select **Apply Changes**

## Results

Once the Action is added, Pangea APIs will be used to perform ip intel checks on new user account creation flows.
The user will either be allowed to continue, or denied. The results of any action will be written to Pangea Secure Audit Log.

## Troubleshooting

For any questions or comments, [reach out to us at Pangea](mailto:integrations@pangea.cloud).
