---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swan.io
  spf: true
  spf_record: v=spf1 include:amazonses.com include:spf.mailjet.com include:_spf.google.com include:spf.mandrillapp.com include:stspg-customer.com include:8668360.spf02.hubspotemail.net include:mail.zendesk.com include:mailgun.org ~all
hosts:
- cert_expires: Aug 16 15:10:30 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: swan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.swan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: api.swan.io
  hsts: null
  https: true
  note: GraphQL API host; returns HTTP 404 to a bare GET (endpoints respond to POST).
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: oauth.swan.io
  hsts: null
  https: true
  note: OAuth2 token host; returns HTTP 404 to a bare GET.
  tls_version: TLSv1.3
- cert_expires: Sep 17 01:37:19 2026 GMT
  cert_issuer: Let's Encrypt (YE1)
  host: docs.swan.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swan Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swan, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swan
provider_slug: swan-io
slug: swan-io-domain-security
source_filename: swan-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + GraphQL/OAuth hosts\nhosts:\n- host: swan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:10:30 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.swan.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.swan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M04\n  hsts: null\n  note: GraphQL API host; returns HTTP 404 to a bare GET (endpoints respond to POST).\n- host: oauth.swan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M04\n  hsts: null\n  note: OAuth2 token host; returns HTTP 404 to a bare GET.\n- host: docs.swan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:37:19 2026 GMT\n  cert_issuer: Let's Encrypt (YE1)\n\
  \  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swan.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:amazonses.com include:spf.mailjet.com include:_spf.google.com include:spf.mandrillapp.com include:stspg-customer.com include:8668360.spf02.hubspotemail.net include:mail.zendesk.com include:mailgun.org ~all'\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/security/swan-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded Banking
- Banking as a Service
- BaaS
- Payments
- Accounts
- Cards
- IBAN
- SEPA
- Europe
- France
- Fintech
- GraphQL
---
