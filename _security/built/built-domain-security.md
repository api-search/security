---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getbuilt.com
  spf: true
hosts:
- cert_expires: Sep 13 09:14:33 2026 GMT
  host: getbuilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Built Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Built, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Built
provider_slug: built
slug: built-domain-security
source_filename: built-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbuilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getbuilt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/built/refs/heads/main/security/built-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction Tech
- Construction Finance
- Real Estate Finance
- Fintech
- Lending
- Payments
- Loan Administration
- Compliance
---
