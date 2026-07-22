---
api_specs:
- filename: vooma-openapi-original.json
  format: json
  label: Vooma Public API
  slug: vooma-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vooma/refs/heads/main/openapi/vooma-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vooma.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vooma.ai
  spf: true
hosts:
- cert_expires: Sep 30 23:02:05 2026 GMT
  host: www.vooma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:55:03 2026 GMT
  host: docs.vooma.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: api.vooma.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vooma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vooma, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vooma
provider_slug: vooma
slug: vooma-domain-security
source_filename: vooma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vooma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.vooma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:55:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vooma.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: vooma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: vooma.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vooma/refs/heads/main/security/vooma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Freight
- Logistics
- Transportation
- Brokers
- TMS
- Agents
---
