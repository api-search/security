---
api_specs:
- filename: mailmodo-openapi.yml
  format: yaml
  label: Mailmodo REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailmodo.com
  spf: true
hosts:
- cert_expires: Sep 21 21:48:54 2026 GMT
  host: www.mailmodo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: manage.mailmodo.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.mailmodo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailmodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailmodo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mailmodo
provider_slug: mailmodo
slug: mailmodo-domain-security
source_filename: mailmodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: manage.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: api.mailmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: mailmodo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/security/mailmodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email
- Interactive Email
- AMP for Email
- Marketing Automation
- Transactional Email
- Campaigns
- Journeys
- Customer Engagement
---
