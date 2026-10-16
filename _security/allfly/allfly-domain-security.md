---
api_specs:
- filename: allfly-openapi-generated.yml
  format: yaml
  label: AllFly API
  slug: allfly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allfly/refs/heads/main/openapi/_ae-authored/allfly-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allfly.io
  spf: true
hosts:
- cert_expires: Dec 13 05:01:11 2026 GMT
  host: allfly.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allfly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AllFly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AllFly
provider_slug: allfly
slug: allfly-domain-security
source_filename: allfly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allfly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 05:01:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allfly.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allfly/refs/heads/main/security/allfly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- CorporateTravel
- Marketplace
- Booking
- SaaS
---
