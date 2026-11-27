---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inite-studio-openapi-generated.yml
  format: yaml
  label: INITE Studio API
  slug: inite-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inite-studio/openapi/_ae-authored/inite-studio-openapi-generated.yml
auth_types: []
description: Authentication methods for INITE Studio
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: INITE Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: INITE Studio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: INITE Studio
provider_slug: inite-studio
scheme_count: 1
schemes:
- evidence: The MCP server uses bearer-token auth — one key per Claude client (laptop, workstation, CI).
  header: Authorization
  how_to_obtain: Generate an API key in Settings → API keys; the plaintext key is shown once and must be copied.
  location: header
  name: API key
  type: http-bearer
slug: inite-studio-authentication
source_filename: inite-studio-authentication.yml
source_heading: Authentication Profile
source_url: https://auth.inite.ai/login?client_id=ideaudit-dashboard&redirect_uri=https%3A%2F%2Fapp.inite.studio%2Fcallback&scope=openid+profile+email+offline_access&state=n-s08aaEcRSFsAWnFddSO4NS-oKitK0K&code_challenge=cYgzAsogfd-ikr_x0vc05hm9-2xKxFwzzvKz5HjtARA&code_challenge_method=S256&nonce=QTfAt5_oYIiTcTtBcOZKWQ04Y1aVYLyJ
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://auth.inite.ai/login?client_id=ideaudit-dashboard&redirect_uri=https%3A%2F%2Fapp.inite.studio%2Fcallback&scope=openid+profile+email+offline_access&state=n-s08aaEcRSFsAWnFddSO4NS-oKitK0K&code_challenge=cYgzAsogfd-ikr_x0vc05hm9-2xKxFwzzvKz5HjtARA&code_challenge_method=S256&nonce=QTfAt5_oYIiTcTtBcOZKWQ04Y1aVYLyJ\nsources:\n- https://auth.inite.ai/login?client_id=ideaudit-dashboard&redirect_uri=https%3A%2F%2Fapp.inite.studio%2Fcallback&scope=openid+profile+email+offline_access&state=n-s08aaEcRSFsAWnFddSO4NS-oKitK0K&code_challenge=cYgzAsogfd-ikr_x0vc05hm9-2xKxFwzzvKz5HjtARA&code_challenge_method=S256&nonce=QTfAt5_oYIiTcTtBcOZKWQ04Y1aVYLyJ\n- https://inite.studio/en/docs/key\n- https://auth.inite.ai/login?client_id=ideaudit-dashboard&redirect_uri=https%3A%2F%2Fapp.inite.studio%2Fcallback&scope=openid+profile+email+offline_access&state=42ziceZMQgfPEKb5wa4EpFpqQaKMdF1z&code_challenge=TXasVOYy1YO6xRNLZoAFQ1jdAxHyrlXVEZhj-XJg0VU&code_challenge_method=S256&nonce=-H959nh_w6Dg_mRb5_60Wo3fAubdiqwW\n\
  description: Authentication methods for INITE Studio\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: The MCP server uses bearer-token auth — one key per Claude client (laptop, workstation, CI).\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in Settings → API keys; the plaintext key is shown once and must be copied.\nnote: No OAuth flows or other authentication schemes are documented on the provided pages.\ndocs: https://auth.inite.ai/login?client_id=ideaudit-dashboard&redirect_uri=https%3A%2F%2Fapp.inite.studio%2Fcallback&scope=openid+profile+email+offline_access&state=n-s08aaEcRSFsAWnFddSO4NS-oKitK0K&code_challenge=cYgzAsogfd-ikr_x0vc05hm9-2xKxFwzzvKz5HjtARA&code_challenge_method=S256&nonce=QTfAt5_oYIiTcTtBcOZKWQ04Y1aVYLyJ\n"
source_yaml_url: https://artifacts.apis.io/inite-studio/authentication/inite-studio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Startups
- Audit
- Analytics
---
