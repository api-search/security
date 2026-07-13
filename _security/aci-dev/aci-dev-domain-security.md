---
api_specs:
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Apps API
  slug: aci-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Functions API
  slug: aci-dev-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev App Configurations API
  slug: aci-dev-app-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
- filename: aci-dev-openapi.yml
  format: yaml
  label: ACI.dev Linked Accounts API
  slug: aci-dev-linked-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/openapi/aci-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aci.dev
  spf: false
hosts:
- cert_expires: Sep 27 19:31:43 2026 GMT
  host: aci.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.aci.dev
  https: false
kind: domain-security
layout: security
method: probed
name: Aci Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACI.dev, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: ACI.dev
provider_slug: aci-dev
slug: aci-dev-domain-security
source_filename: aci-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aci.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:31:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.aci.dev\n  https: false\ndomains:\n- domain: aci.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aci-dev/refs/heads/main/security/aci-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agent Infrastructure
- Agents
- AI
- Artificial Intelligence
- Function Calling
- MCP
- Model Context Protocol
- OAuth
- Open Source
- Tool Calling
- VibeOps
---
