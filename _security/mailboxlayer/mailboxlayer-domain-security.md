---
api_specs:
- filename: mailboxlayer-openapi.yml
  format: yaml
  label: mailboxlayer Verification API
  slug: mailboxlayer-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/openapi/mailboxlayer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mailboxlayer.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apilayer.net
  spf: true
hosts:
- cert_expires: Oct  2 07:32:28 2026 GMT
  host: mailboxlayer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: apilayer.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailboxlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailboxlayer, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mailboxlayer
provider_slug: mailboxlayer
slug: mailboxlayer-domain-security
source_filename: mailboxlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailboxlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:32:28 2026 GMT\n  hsts: false\n- host: apilayer.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: mailboxlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apilayer.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/security/mailboxlayer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Email Verification
- Email Validation
- SMTP
- MX Records
- Catch-All Detection
- Disposable Email
- Free Email Provider
- Role Address
- Quality Score
- apilayer
- Public APIs
---
