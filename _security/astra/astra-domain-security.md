---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: astra.finance
  spf: true
hosts:
- cert_expires: Sep 18 13:53:42 2026 GMT
  host: docs.astra.finance
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 22:42:41 2026 GMT
  host: api.astra.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Astra
provider_slug: astra
slug: astra-domain-security
source_filename: astra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.astra.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 13:53:42 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.astra.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:42:41 2026 GMT\n  hsts: null\ndomains:\n- domain: astra.finance\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astra/refs/heads/main/security/astra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Fintech
- Money Movement
- ACH
- Instant Payments
- Bank Transfers
- Disbursements
- API
---
