---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for MeshKore unified API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MeshKore Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeshKore declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MeshKore
provider_slug: meshkore-com
scheme_count: 1
schemes:
- evidence: 'DELETE /v1/agents/me Authorization: Bearer <token>'
  header: Authorization
  how_to_obtain: 'TOKEN=$(curl -s -X POST https://api.meshkore.com/v1/agents/token \ -H ''content-type: application/json'' \ -d ''{"agent_id":"<your-agent-id>","api_key":"<your-api-key>"}'' \ | jq -r .token)'
  location: header
  name: Bearer
  type: http-bearer
slug: meshkore-com-authentication
source_filename: meshkore-com-authentication.yml
source_heading: Authentication Profile
source_url: https://meshkore.com/reference/standards/stack/apis.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://meshkore.com/reference/standards/stack/apis.md\nsources:\n- https://meshkore.com/reference/standards/stack/apis.md\n- https://meshkore.com/reference/agents/deregister.md\n- https://meshkore.com/reference/agents/clusters.md\n- https://meshkore.com/reference/cluster/onboarding/deploy-bot.md.template\ndescription: Authentication schemes for MeshKore unified API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'DELETE /v1/agents/me Authorization: Bearer <token>'\n  location: header\n  header: Authorization\n  how_to_obtain: 'TOKEN=$(curl -s -X POST https://api.meshkore.com/v1/agents/token \\ -H ''content-type: application/json'' \\ -d ''{\"agent_id\":\"<your-agent-id>\",\"api_key\":\"<your-api-key>\"}''\n    \\ | jq -r .token)'\ndocs: https://meshkore.com/reference/standards/stack/apis.md\n"
source_yaml_url: https://artifacts.apis.io/meshkore-com/authentication/meshkore-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Infrastructure
- Open Source
- Cloudflare
- Autonomous Agents
---
