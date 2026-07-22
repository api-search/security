---
api_specs:
- filename: qentaz-webhooks-asyncapi.yml
  format: yaml
  label: Trazo API
  slug: trazo-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/qentaz/refs/heads/main/asyncapi/qentaz-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - bfeb96f7e8fae3a5.vercel-dns-016.com.
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: trazo.co
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: qentaz.com
  spf: true
hosts:
- cert_expires: Oct  6 10:50:05 2026 GMT
  host: www.trazo.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 03:27:56 2026 GMT
  host: docs.qentaz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.qentaz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qentaz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qentaz, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Qentaz
provider_slug: qentaz
slug: qentaz-domain-security
source_filename: qentaz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trazo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:50:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qentaz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 03:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.qentaz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: trazo.co\n  dnssec: true\n  caa:\n  - bfeb96f7e8fae3a5.vercel-dns-016.com.\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: qentaz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qentaz/refs/heads/main/security/qentaz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Collections
- Disbursements
- Reconciliation
- Fintech
- Colombia
- Webhooks
- Fraud Prevention
- WhatsApp Payments
---
