---
api_specs:
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey
  slug: portkey
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey Inference API
  slug: portkey-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
- filename: portkey-openapi.yml
  format: yaml
  label: Portkey Admin API
  slug: portkey-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/openapi/portkey-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: portkey.ai
  spf: true
hosts:
- cert_expires: Oct  6 08:44:14 2026 GMT
  host: portkey.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:14:05 2026 GMT
  host: api.portkey.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portkey, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Portkey
provider_slug: portkey
slug: portkey-domain-security
source_filename: portkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portkey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:44:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.portkey.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:14:05 2026 GMT\n  hsts: null\ndomains:\n- domain: portkey.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portkey/refs/heads/main/security/portkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateways
- Gateways
- Governance
- Guardrails
- Observability
- Prompt Management
---
