---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods documented for Jiminny integrations
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jiminny Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jiminny declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Jiminny
provider_slug: jiminny
scheme_count: 2
schemes:
- evidence: b. Once installation is complete, you'll need to connect with your Jiminny instance. This is done by entering your bearer token key and selecting the Jiminny environment.
  header: Authorization
  how_to_obtain: Retrieve the token/API key from Jiminny > Settings > Integrations.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Paste your Bearer token provided into the `Authorization` header
  header: Authorization
  how_to_obtain: Provided by Jiminny Engineering when a SCIM endpoint is requested via a Service Request (SRD) ticket.
  location: header
  name: SCIM Bearer token
  type: http-bearer
slug: jiminny-authentication
source_filename: jiminny-authentication.yml
source_heading: Authentication Profile
source_url: https://help.jiminny.com/en/articles/9529066-jiminny-salesforce-application-admin-setup.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.jiminny.com/en/articles/9529066-jiminny-salesforce-application-admin-setup.md\nsources:\n- https://help.jiminny.com/en/articles/9529066-jiminny-salesforce-application-admin-setup.md\n- https://help.jiminny.com/en/articles/9528966-scim-setup-guide.md\n- https://help.jiminny.com/en/articles/3350614-inbound-calling-setup.md\n- https://help.jiminny.com/en/articles/1567290-getting-started-with-sms.md\ndescription: Authentication methods documented for Jiminny integrations\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: b. Once installation is complete, you'll need to connect with your Jiminny instance. This is done by entering your bearer token key\n    and selecting the Jiminny environment.\n  location: header\n  header: Authorization\n  how_to_obtain: Retrieve the token/API key from Jiminny > Settings > Integrations.\n- type: http-bearer\n  name: SCIM\
  \ Bearer token\n  evidence: Paste your Bearer token provided into the `Authorization` header\n  location: header\n  header: Authorization\n  how_to_obtain: Provided by Jiminny Engineering when a SCIM endpoint is requested via a Service Request (SRD) ticket.\ndocs: https://help.jiminny.com/en/articles/9529066-jiminny-salesforce-application-admin-setup.md\n"
source_yaml_url: https://artifacts.apis.io/jiminny/authentication/jiminny-authentication.yml
summary_line: 2 schemes
tags:
- Sales Intelligence
- Artificial Intelligence
- Revenue
- CRM Integration
- Analytics
---
