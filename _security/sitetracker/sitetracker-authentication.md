---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Sitetracker Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sitetracker declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Sitetracker
provider_slug: sitetracker
scheme_count: 3
schemes:
- evidence: https://community.sitetracker.com/ 302s to https://login.salesforce.com/setup/secur/RemoteAccessAuthorizationPage.apexp — the Salesforce OAuth connected-app authorization page.
  flows_documented_by: https://help.salesforce.com/ (Salesforce, not Sitetracker)
  id: salesforce-oauth2
  name: Salesforce OAuth 2.0 (connected app)
  observed: true
  type: oauth2
- evidence: https://help.sitetracker.com/ serves a login page whose only action is GET /oauth2/authorization/salesforce.
  id: salesforce-oauth2-app
  name: Salesforce OAuth 2.0 (Sitetracker EDU application)
  observed: true
  type: oauth2
- evidence: https://sitetracker-login.cloudforce.com/ (HTTP 200) is the customer-facing Salesforce My Domain login linked from the sitetracker.com header.
  id: salesforce-session
  name: Salesforce session ID / My Domain login
  observed: true
  scheme: session
  type: http
slug: sitetracker-authentication
source_filename: sitetracker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  Observed redirect chains on https://help.sitetracker.com/ and\n  https://community.sitetracker.com/; https://sitetracker-login.cloudforce.com/;\n  https://www.sitetracker.com/products-services/integrations/\nnote: >-\n  DERIVED FROM NOTHING WOULD BE A GUESS — this profile is built from what the\n  live hosts actually did, not from a spec (Sitetracker publishes none) and not\n  from an auth docs page (Sitetracker publishes none publicly). Sitetracker\n  operates no authorization server of its own: authentication is delegated\n  wholly to Salesforce. Every Sitetracker property that requires a credential\n  hands off to a Salesforce OAuth 2.0 connected-app flow, and the customer's API\n  credentials are Salesforce org credentials, not Sitetracker-issued ones. The\n  scope reference, token lifetimes and connected-app configuration are therefore\n  Salesforce's, and the Sitetracker-specific object permissions sit behind the\n\
  \  customer login. No `scopes/` artifact is written: Sitetracker documents no\n  scope surface of its own.\ndelegated_to: Salesforce\nauthorization_server_operated_by_provider: false\nschemes:\n- id: salesforce-oauth2\n  type: oauth2\n  name: Salesforce OAuth 2.0 (connected app)\n  observed: true\n  evidence: >-\n    https://community.sitetracker.com/ 302s to\n    https://login.salesforce.com/setup/secur/RemoteAccessAuthorizationPage.apexp —\n    the Salesforce OAuth connected-app authorization page.\n  flows_documented_by: https://help.salesforce.com/ (Salesforce, not Sitetracker)\n- id: salesforce-oauth2-app\n  type: oauth2\n  name: Salesforce OAuth 2.0 (Sitetracker EDU application)\n  observed: true\n  evidence: >-\n    https://help.sitetracker.com/ serves a login page whose only action is\n    GET /oauth2/authorization/salesforce.\n- id: salesforce-session\n  type: http\n  scheme: session\n  name: Salesforce session ID / My Domain login\n  observed: true\n  evidence: >-\n    https://sitetracker-login.cloudforce.com/\
  \ (HTTP 200) is the customer-facing\n    Salesforce My Domain login linked from the sitetracker.com header.\npublic_auth_documentation: false\npublic_auth_documentation_note: >-\n  Sitetracker publishes no public authentication guide. The integrations page\n  states the APIs are the Salesforce REST/SOAP/Bulk APIs but links no auth\n  reference of its own.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sitetracker/refs/heads/main/authentication/sitetracker-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Telecommunications
- Utilities
- Energy
- EV Charging
- Fiber Networks
- Asset Management
- Project Management
- Field Service
- Salesforce
- Critical Infrastructure
---
