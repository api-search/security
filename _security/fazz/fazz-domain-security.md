---
api_specs:
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Accept API (Singapore)
  slug: fazz-accept-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Send API (Singapore)
  slug: fazz-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
- filename: fazz-openapi.yml
  format: yaml
  label: Fazz Payment Methods API
  slug: fazz-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/openapi/fazz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc@smtp.mailtrap.live; ruf=mailto:dmarc@smtp.mailtrap.live; rf=afrf; pct=100
  dnssec: false
  domain: fazz.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:_spf.smtp.mailtrap.live ~all
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:enablethisnexttime@xfers.io
  dnssec: false
  domain: xfers.io
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mailgun.org ~all
hosts:
- cert_expires: Aug 23 03:38:06 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: www.xfers.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  notes: Production Fazz Payments API host (base path /api/v4).
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:17:40 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: fazz.com
  hsts: false
  https: true
  notes: Corporate/marketing site; no HSTS header observed on the root response.
  tls_version: TLSv1.3
- cert_expires: Aug 29 07:54:17 2026 GMT
  cert_issuer: Let's Encrypt (YE2)
  host: docs.fazz.com
  https: true
  notes: Developer documentation portal.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fazz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fazz, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fazz
provider_slug: fazz
slug: fazz-domain-security
source_filename: fazz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xfers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Aug 23 03:38:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  notes: Production Fazz Payments API host (base path /api/v4).\n- host: fazz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 23 07:17:40 2026 GMT\n  hsts: false\n  notes: Corporate/marketing site; no HSTS header observed on the root response.\n- host: docs.fazz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE2)\n  cert_expires: Aug 29 07:54:17 2026 GMT\n  notes: Developer documentation portal.\ndomains:\n- domain: fazz.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:mail.zendesk.com include:_spf.smtp.mailtrap.live\
  \ ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; rua=mailto:dmarc@smtp.mailtrap.live; ruf=mailto:dmarc@smtp.mailtrap.live; rf=afrf; pct=100'\n- domain: xfers.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:_spf.google.com include:mailgun.org ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: 'v=DMARC1; p=quarantine; rua=mailto:enablethisnexttime@xfers.io'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fazz/refs/heads/main/security/fazz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Payments
- Business Banking
- Disbursements
- Southeast Asia
- PayNow
- Virtual Accounts
---
