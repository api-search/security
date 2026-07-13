---
api_specs:
- filename: firstpromoter-firstpromoter-admin-api-openapi.yml
  format: yaml
  label: FirstPromoter Admin API
  slug: firstpromoter-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/openapi/firstpromoter-firstpromoter-admin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: firstpromoter.com
  spf: true
hosts:
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: firstpromoter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: docs.firstpromoter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 10:07:09 2026 GMT
  host: api.firstpromoter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firstpromoter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirstPromoter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FirstPromoter
provider_slug: firstpromoter
slug: firstpromoter-domain-security
source_filename: firstpromoter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.firstpromoter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:07:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: firstpromoter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firstpromoter/refs/heads/main/security/firstpromoter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Referral Tracking
- SaaS
- Commission Management
- Reward Distribution
- Promoters
---
