---
api_specs:
- filename: openapi.json
  format: json
  label: Zoho Mail API
  slug: zoho-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoho.eu
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.zoho.com
  hsts: true
  hsts_max_age: 64072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: mail.zoho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: mail.zoho.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoho Mail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoho Mail, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoho Mail
provider_slug: zoho-mail
slug: zoho-mail-domain-security
source_filename: zoho-mail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 64072000\n- host: mail.zoho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\n- host: mail.zoho.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zoho.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zoho.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-mail/refs/heads/main/security/zoho-mail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Mail
- Collaboration
- Messaging
- Calendar
- Contacts
- Organization Management
- SaaS
---
