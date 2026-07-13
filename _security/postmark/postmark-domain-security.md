---
api_specs:
- filename: postmark-api-openapi.yml
  format: yaml
  label: Postmark API
  slug: postmark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postmark/refs/heads/main/openapi/postmark-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: postmarkapp.com
  spf: true
hosts:
- cert_expires: Sep 23 13:18:46 2026 GMT
  host: postmarkapp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.postmarkapp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postmark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postmark, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Postmark
provider_slug: postmark
slug: postmark-domain-security
source_filename: postmark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postmarkapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:18:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.postmarkapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: postmarkapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postmark/refs/heads/main/security/postmark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Emails
- Messaging
- Transactional Email
- Deliverability
- SMTP
---
