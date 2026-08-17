---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Oneshot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OneShot secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OneShot
provider_slug: oneshot
scheme_count: 3
schemes:
- audience: OneShot UI -> OneShot backend
  bearerFormat: JWT
  evidence: '"Once the user logs-in to Oneshot through Salesforce login, Oneshot issues a JWT token which expires in 60 minutes ... This is going to be used as an authorization token which will authorize the user to make API calls against the Oneshot system from Oneshot User interface (UI)."'
  issued_by: OneShot, after Salesforce login
  name: platformJwt
  role: server
  scheme: bearer
  source: https://www.oneshot.ai/handlingdata
  ttl_seconds: 3600
  type: http
- evidence: '"A user is created in the Oneshot system with the users email address, username and OAuth access tokens. This allows Oneshot to make secure API calls against the users CRM account. OneShot adheres to industry standard security practices defined by Salesforce''s official OAuth process."'
  flow: authorizationCode
  name: salesforceOAuth
  provider: Salesforce
  provider_docs: https://help.salesforce.com/articleView?id=remoteaccess_oauth_flows.htm&type=5
  role: client
  source: https://www.oneshot.ai/handlingdata
  type: oauth2
- evidence: '"A user connects their Outreach''s account or Email account(Gmail or Outlook) with Oneshot. This is secured by industry standard OAuth process and Oneshot stores the access tokens to be able to make API calls to Outreach and/or email on the user''s behalf."'
  flow: authorizationCode
  name: outreachEmailOAuth
  provider: Outreach / Gmail / Outlook
  role: client
  source: https://www.oneshot.ai/handlingdata
  type: oauth2
slug: oneshot-authentication
source_filename: oneshot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.oneshot.ai/handlingdata\nscope: internal-platform\npointer_emitted: false\nnote: >-\n  READ THIS BEFORE WIRING A POINTER. This file documents the auth model of OneShot's OWN\n  application — the browser UI talking to its own backend — as described in OneShot's\n  published \"Guide to Handling of Customer Data\". It is NOT a developer-facing API\n  authentication reference, because OneShot publishes no developer API: there is no\n  reference page, no key issuance flow, and no reachable API host. Therefore NO\n  `Authentication` pointer is emitted in apis.yml. Emitting one would earn the\n  authentication_documented ergonomics check for documentation that no integrator can act\n  on. Captured anyway because it is real, provider-published, and it is the only technical\n  description of OneShot's auth posture that exists.\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  bearer_format: JWT\n  oauth2_role:\
  \ client\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: platformJwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  role: server\n  ttl_seconds: 3600\n  issued_by: OneShot, after Salesforce login\n  audience: OneShot UI -> OneShot backend\n  evidence: >-\n    \"Once the user logs-in to Oneshot through Salesforce login, Oneshot issues a JWT token\n    which expires in 60 minutes ... This is going to be used as an authorization token which\n    will authorize the user to make API calls against the Oneshot system from Oneshot User\n    interface (UI).\"\n  source: https://www.oneshot.ai/handlingdata\n- name: salesforceOAuth\n  type: oauth2\n  role: client\n  flow: authorizationCode\n  provider: Salesforce\n  evidence: >-\n    \"A user is created in the Oneshot system with the users email address, username and\n    OAuth access tokens. This allows Oneshot to make secure API calls against the users CRM\n    account. OneShot adheres to industry standard security\
  \ practices defined by Salesforce's\n    official OAuth process.\"\n  provider_docs: https://help.salesforce.com/articleView?id=remoteaccess_oauth_flows.htm&type=5\n  source: https://www.oneshot.ai/handlingdata\n- name: outreachEmailOAuth\n  type: oauth2\n  role: client\n  flow: authorizationCode\n  provider: Outreach / Gmail / Outlook\n  evidence: >-\n    \"A user connects their Outreach's account or Email account(Gmail or Outlook) with\n    Oneshot. This is secured by industry standard OAuth process and Oneshot stores the\n    access tokens to be able to make API calls to Outreach and/or email on the user's behalf.\"\n  source: https://www.oneshot.ai/handlingdata\ntoken_handling:\n  downstream_tokens_exposed_to_client: false\n  evidence: 'None of those access tokens are exposed to the clients.'\n  storage: MongoDB Atlas (OneShot cloud), access limited to approved designated employees\n  transport: SSL/HTTPS for all network traffic\nbackend_host:\n  host: api.oneshot.ai\n  resolves: false\n\
  \  note: >-\n    The app.oneshot.ai JavaScript bundle references https://api.oneshot.ai as the platform\n    backend, but the host has no public DNS record (NOERROR/ANSWER:0 from both 8.8.8.8 and\n    1.1.1.1). Recorded as an observation about reachability; NOT written to apis.yml as a\n    baseURL, because a host that does not resolve is not a base URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oneshot/refs/heads/main/authentication/oneshot-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Sales
- Sales Automation
- Outbound
- Prospecting
- Lead Generation
- Artificial Intelligence
- Go-To-Market
---
