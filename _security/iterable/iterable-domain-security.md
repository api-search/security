---
api_specs:
- filename: iterable-rest-api-openapi.yml
  format: yaml
  label: Iterable REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-rest-api-openapi.yml
- filename: iterable-export-api-openapi.yml
  format: yaml
  label: Iterable Export API
  slug: export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/openapi/iterable-export-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iterable.com
  spf: true
hosts:
- cert_expires: Sep 14 20:55:23 2026 GMT
  host: iterable.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: api.iterable.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  1 23:46:40 2026 GMT
  host: support.iterable.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iterable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iterable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Iterable
provider_slug: iterable
slug: iterable-domain-security
source_filename: iterable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iterable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.iterable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: support.iterable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:46:40 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: iterable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iterable/refs/heads/main/security/iterable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cross-Channel Messaging
- Customer Engagement
- Email
- Marketing Automation
- Push Notifications
- SMS
---
