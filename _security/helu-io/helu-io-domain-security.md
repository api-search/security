---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helu.io
  spf: true
hosts:
- cert_expires: Oct  2 08:47:04 2026 GMT
  host: helu.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helu Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helu Io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Helu Io
provider_slug: helu-io
slug: helu-io-domain-security
source_filename: helu-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helu.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:47:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helu.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helu-io/refs/heads/main/security/helu-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial
- Controlling
- Reporting
- Analytics
- Accounting
- DATEV
- FinTech
- Business Intelligence
- SME
---
