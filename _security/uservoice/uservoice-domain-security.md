---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: UserVoice Admin API
  slug: uservoice-admin-api
  spec_type: OpenAPI
  url: https://developer.uservoice.com/docs/api/v2/reference/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uservoice.com
  spf: true
hosts:
- cert_expires: Sep 19 21:29:37 2026 GMT
  host: www.uservoice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:45 2026 GMT
  host: developer.uservoice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:00:45 2026 GMT
  host: subdomain.uservoice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uservoice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UserVoice, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: UserVoice
provider_slug: uservoice
slug: uservoice-domain-security
source_filename: uservoice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uservoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:29:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.uservoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: subdomain.uservoice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:00:45 2026 GMT\n  hsts: null\ndomains:\n- domain: uservoice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uservoice/refs/heads/main/security/uservoice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Product Feedback
- Idea Management
- Customer Feedback
- Product Roadmap
- Voting
- Feature Requests
- User Research
- SaaS
---
