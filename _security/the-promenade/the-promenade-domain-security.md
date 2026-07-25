---
api_specs:
- filename: the-promenade-payments-api-openapi.yml
  format: yaml
  label: The Promenade payments API
  slug: the-promenade-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-promenade/refs/heads/main/openapi/the-promenade-payments-api-openapi.yml
- filename: the-promenade-session-api-openapi.yml
  format: yaml
  label: The Promenade session API
  slug: the-promenade-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-promenade/refs/heads/main/openapi/the-promenade-session-api-openapi.yml
- filename: the-promenade-signup-api-openapi.yml
  format: yaml
  label: The Promenade signup API
  slug: the-promenade-signup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-promenade/refs/heads/main/openapi/the-promenade-signup-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simcluster.ai
  spf: true
hosts:
- cert_expires: Sep  2 10:18:20 2026 GMT
  host: simcluster.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Promenade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Promenade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Promenade
provider_slug: the-promenade
slug: the-promenade-domain-security
source_filename: the-promenade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simcluster.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:18:20 2026 GMT\n  hsts: false\ndomains:\n- domain: simcluster.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-promenade/refs/heads/main/security/the-promenade-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- MCP
- Media Generation
- Social Network
- Generative AI
- Gaming
---
