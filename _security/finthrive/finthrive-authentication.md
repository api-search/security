---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Finthrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: FinThrive declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: FinThrive
provider_slug: finthrive
scheme_count: 0
schemes: []
slug: finthrive-authentication
source_filename: finthrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://api-portal.nthrive.com/ + https://api-portal.nthrive.com/signin\napi_auth_documented_publicly: false\nnote: >-\n  No Authentication pointer is wired in apis.yml. This file records what can be observed\n  about identity on FinThrive's API surface, and what can be observed is PORTAL identity,\n  not the API's own security scheme. FinThrive publishes no OpenAPI, so\n  0-working/derive-authentication.py has nothing to read; and the developer portal's own\n  catalog endpoint returns zero APIs anonymously, so the security schemes attached to\n  those APIs cannot be seen without credentials. Asserting an Authentication artifact\n  here would credit FinThrive with documented auth it has not published.\nportal_identity:\n  host: https://api-portal.nthrive.com\n  platform: Microsoft Azure API Management developer portal\n  providers:\n  - name: Azure Active Directory\n    path: /signin\n    note: 'Portal text: \"Users with Azure\
  \ Active Directory credentials sign in here.\"'\n  - name: FinThrive evaluation credentials\n    path: /evalsignin\n    note: 'Portal text: \"If you have received credentials from FinThrive, use Evaluation Sign in, then go to the Products page.\"'\napi_identity:\n  scheme: unknown\n  note: >-\n    Azure API Management's default subscription-key model (Ocp-Apim-Subscription-Key)\n    is the platform norm and the portal's \"sign up to acquire keys\" boilerplate is\n    consistent with it, but FinThrive publishes nothing confirming it, so no scheme is\n    asserted here.\n  discovery_probes:\n  - {url: 'https://api.finthrive.com/.well-known/openid-configuration', status: 404}\n  - {url: 'https://api.finthrive.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://api.finthrive.com/.well-known/oauth-protected-resource', status: 404}\n  - {url: 'https://api-portal.nthrive.com/mapi/apis?api-version=2022-08-01', status: 200, body: '{\"value\":[],\"count\":0}'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finthrive/refs/heads/main/authentication/finthrive-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Healthcare
- Revenue Cycle Management
- Health IT
- Claims
- Billing
- Payments
- Insurance
- Patient Access
- Analytics
- Software-as-a-Service
- United States
---
