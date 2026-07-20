---
api_specs:
- filename: agora-openapi-original.yml
  format: yaml
  label: Agora Public API
  slug: agora-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/openapi/agora-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agora.finance
  spf: true
hosts:
- cert_expires: Sep 24 16:31:06 2026 GMT
  host: docs.agora.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:28:46 2026 GMT
  host: api.agora.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agora, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agora
provider_slug: agora
slug: agora-domain-security
source_filename: agora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.agora.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.agora.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:28:46 2026 GMT\n  hsts: null\ndomains:\n- domain: agora.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agora/refs/heads/main/security/agora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Stablecoin
- Digital Dollar
- Payments
- Cryptocurrency
- Blockchain
- API
- AUSD
---
