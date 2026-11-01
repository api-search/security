---
anonymous_access: false
api_key_in: []
auth_types: []
description: Twain connects to HubSpot using OAuth. The user clicks Connect, is sent to HubSpot’s approval screen, signs in, chooses an account, and approves the requested scopes. Twain then receives an access token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Twain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twain declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Twain
provider_slug: twain
scheme_count: 1
schemes:
- evidence: Clicking Connect sends you to HubSpot's own approval screen. Sign in if you are not already, choose the account you want to connect, and review the permissions Twain is asking for.
  flows:
  - authorization_code
  how_to_obtain: User initiates connection in Twain, is redirected to HubSpot’s OAuth approval screen, approves scopes, and Twain receives the access token.
  name: OAuth
  scopes:
  - oauth
  - crm.objects.contacts.read
  - crm.objects.contacts.write
  - crm.schemas.contacts.read
  - crm.schemas.contacts.write
  - crm.lists.read
  - sales-email-read
  - crm.objects.deals.read
  - crm.objects.companies.read
  type: oauth2
slug: twain-authentication
source_filename: twain-authentication.yml
source_heading: Authentication Profile
source_url: https://www.twain.ai/blog/hubspot-setup-guide
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.twain.ai/blog/hubspot-setup-guide\nsources:\n- https://www.twain.ai/blog/hubspot-setup-guide\ndescription: Twain connects to HubSpot using OAuth. The user clicks Connect, is sent to HubSpot’s approval screen, signs in, chooses an account,\n  and approves the requested scopes. Twain then receives an access token.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Clicking Connect sends you to HubSpot's own approval screen. Sign in if you are not already, choose the account you want to connect,\n    and review the permissions Twain is asking for.\n  flows:\n  - authorization_code\n  scopes:\n  - oauth\n  - crm.objects.contacts.read\n  - crm.objects.contacts.write\n  - crm.schemas.contacts.read\n  - crm.schemas.contacts.write\n  - crm.lists.read\n  - sales-email-read\n  - crm.objects.deals.read\n  - crm.objects.companies.read\n  how_to_obtain: User initiates connection\
  \ in Twain, is redirected to HubSpot’s OAuth approval screen, approves scopes, and Twain receives the\n    access token.\ndocs: https://www.twain.ai/blog/hubspot-setup-guide\n"
source_yaml_url: https://artifacts.apis.io/twain/authentication/twain-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Outreach
- Sales
- Marketing
---
