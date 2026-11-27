---
anonymous_access: false
api_key_in: []
auth_types: []
description: OneLence uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: OneLence Authentication
name_suffix: Authentication
oauth_flows: []
overview: OneLence declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: OneLence
provider_slug: onelence-com
scheme_count: 3
schemes:
- evidence: Publishable Keys Used for browser-side tracking through the SDK.
  how_to_obtain: Navigate to Settings → API Keys, select Publishable in the key type selector, enter a name and click Create.
  name: Publishable Key
  type: apiKey
- evidence: Secret Keys Used for server-to-server event transmission.
  how_to_obtain: Navigate to Settings → API Keys, select Secret in the key type selector, enter a name and click Create.
  name: Secret Key
  type: apiKey
- evidence: Webhook Keys Used for validating incoming webhook notifications and integration callbacks.
  how_to_obtain: Navigate to Settings → API Keys, select Webhook in the key type selector, enter a name and click Create.
  name: Webhook Key
  type: apiKey
slug: onelence-com-authentication
source_filename: onelence-com-authentication.yml
source_heading: Authentication Profile
source_url: https://onelence.com/docs/guides/workspace-features/api
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://onelence.com/docs/guides/workspace-features/api\nsources:\n- https://onelence.com/docs/guides/workspace-features/api\n- https://onelence.com/docs/integrations/start-integration\n- https://onelence.com/docs/integrations/advanced-tracking-configuration\n- https://onelence.com/docs/integrations\ndescription: OneLence uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: Publishable Key\n  evidence: Publishable Keys Used for browser-side tracking through the SDK.\n  how_to_obtain: Navigate to Settings → API Keys, select Publishable in the key type selector, enter a name and click Create.\n- type: apiKey\n  name: Secret Key\n  evidence: Secret Keys Used for server-to-server event transmission.\n  how_to_obtain: Navigate to Settings → API Keys, select Secret in the key type selector, enter a name and click Create.\n- type: apiKey\n  name: Webhook Key\n  evidence:\
  \ Webhook Keys Used for validating incoming webhook notifications and integration callbacks.\n  how_to_obtain: Navigate to Settings → API Keys, select Webhook in the key type selector, enter a name and click Create.\ndocs: https://onelence.com/docs/guides/workspace-features/api\n"
source_yaml_url: https://artifacts.apis.io/onelence-com/authentication/onelence-com-authentication.yml
summary_line: 3 schemes
tags:
- Marketing Intelligence
- Affiliate Marketing
- SEO
- AI Visibility
- Growth Analytics
---
