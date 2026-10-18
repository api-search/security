---
anonymous_access: false
api_key_in: []
auth_types: []
description: Classet uses an API key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Classet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Classet declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Classet
provider_slug: classet
scheme_count: 1
schemes:
- evidence: To verify our webhook, your most recent, active api key will be passed in the header as `x-classet-key`.
  header: x-classet-key
  how_to_obtain: Create a new key in Developer Settings in the Classet app.
  location: header
  name: API Key
  type: apiKey
slug: classet-authentication
source_filename: classet-authentication.yml
source_heading: Authentication Profile
source_url: https://help.classet.ai/article/signing-up-when-your-company-already-uses-classet
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.classet.ai/article/signing-up-when-your-company-already-uses-classet\nsources:\n- https://help.classet.ai/article/signing-up-when-your-company-already-uses-classet\n- https://docs.classet.ai/reference/getting-started-with-classet.md\n- https://docs.classet.ai/reference/getting-started-with-classet\ndescription: Classet uses an API key for authentication.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: To verify our webhook, your most recent, active api key will be passed in the header as `x-classet-key`.\n  location: header\n  header: x-classet-key\n  how_to_obtain: Create a new key in Developer Settings in the Classet app.\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://help.classet.ai/article/signing-up-when-your-company-already-uses-classet\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classet/refs/heads/main/authentication/classet-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Recruiting
- Applicant Tracking
- Automation
- Enterprise
---
