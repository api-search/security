---
anonymous_access: false
api_key_in: []
api_specs:
- filename: promptitude-openapi-generated.yml
  format: yaml
  label: Promptitude API
  slug: promptitude-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptitude/openapi/_ae-authored/promptitude-openapi-generated.yml
auth_types: []
description: Promptitude uses API keys for authentication. Include the API key as a Bearer token in the Authorization header of every request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Promptitude Authentication
name_suffix: Authentication
oauth_flows: []
overview: Promptitude declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Promptitude
provider_slug: promptitude
scheme_count: 1
schemes:
- evidence: 'Recommended: Header with Bearer Token With every request you send to the Promptitude API, include an Authorization Header like this: Header Authorization Value Bearer YOUR_API_TOKEN'
  header: Authorization
  how_to_obtain: You can find your default API key in Promptitude's Settings . Just click the little "copy" icon, and paste it into your code.
  location: header
  name: Bearer
  type: http-bearer
slug: promptitude-authentication
source_filename: promptitude-authentication.yml
source_heading: Authentication Profile
source_url: https://help.promptitude.io/en/articles/8890416-ultimate-guide-everything-you-need-to-know-before-adding-your-openai-api-key
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.promptitude.io/en/articles/8890416-ultimate-guide-everything-you-need-to-know-before-adding-your-openai-api-key\nsources:\n- https://help.promptitude.io/en/articles/8890416-ultimate-guide-everything-you-need-to-know-before-adding-your-openai-api-key\n- https://help.promptitude.io/en/articles/8892755-how-to-get-your-api-key-for-openai\n- https://help.promptitude.io/en/articles/8909341-authentication\n- https://help.promptitude.io/en/articles/9682142-where-to-find-your-perplexity-api-key-a-step-by-step-guide\ndescription: Promptitude uses API keys for authentication. Include the API key as a Bearer token in the Authorization header of every request.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Recommended: Header with Bearer Token With every request you send to the Promptitude API, include an Authorization Header like this:\n    Header Authorization Value\
  \ Bearer YOUR_API_TOKEN'\n  location: header\n  header: Authorization\n  how_to_obtain: You can find your default API key in Promptitude's Settings . Just click the little \"copy\" icon, and paste it into your code.\ndocs: https://help.promptitude.io/en/articles/8890416-ultimate-guide-everything-you-need-to-know-before-adding-your-openai-api-key\n"
source_yaml_url: https://artifacts.apis.io/promptitude/authentication/promptitude-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- No-Code
- Prompt Engineering
- Automation
---
