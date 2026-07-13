---
api_specs:
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana AI Assistant & Agents API
  slug: ai-assistant-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Knowledge & Search API
  slug: knowledge-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Learn Content & Learning API
  slug: content-learning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
- filename: sana-labs-openapi.yml
  format: yaml
  label: Sana Integrations API
  slug: integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/openapi/sana-labs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sana.ai
  spf: true
hosts:
- cert_expires: Aug 20 10:25:05 2026 GMT
  host: www.sana.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: docs.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: <domain>.sana.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Sana Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sana, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sana
provider_slug: sana-labs
slug: sana-labs-domain-security
source_filename: sana-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 10:25:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\n- host: <domain>.sana.ai\n  https: false\ndomains:\n- domain: sana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana-labs/refs/heads/main/security/sana-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Knowledge
- Learning
- LMS
- Agents
---
