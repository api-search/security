---
api_specs:
- filename: salesflare-api-openapi.yml
  format: yaml
  label: Salesflare API
  slug: salesflare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesflare/refs/heads/main/openapi/salesflare-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: salesflare.com
  spf: true
hosts:
- cert_expires: Sep 28 06:35:21 2026 GMT
  host: salesflare.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 10:16:35 2026 GMT
  host: api.salesflare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Salesflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesflare, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Salesflare
provider_slug: salesflare
slug: salesflare-domain-security
source_filename: salesflare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salesflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:35:21 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.salesflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 10:16:35 2026 GMT\n  hsts: null\ndomains:\n- domain: salesflare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesflare/refs/heads/main/security/salesflare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- B2B
- Contacts
- Accounts
- Opportunities
- Email
- Automation
- Lead Generation
---
