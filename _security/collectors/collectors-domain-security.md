---
api_specs:
- filename: collectors-psa-openapi-original.json
  format: json
  label: PSA Public API
  slug: psa-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/openapi/collectors-psa-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: collectors.com
  spf: true
hosts:
- cert_expires: Aug 30 03:59:22 2026 GMT
  host: www.collectors.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Collectors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collectors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Collectors
provider_slug: collectors
slug: collectors-domain-security
source_filename: collectors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.collectors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:59:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: collectors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/security/collectors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Collectibles
- Authentication
- Grading
- Trading Cards
- Verification
---
