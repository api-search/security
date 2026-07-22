---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: papernest.com
  spf: true
hosts:
- cert_expires: Sep 21 07:06:13 2026 GMT
  host: www.papernest.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Papernest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Papernest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Papernest
provider_slug: papernest
slug: papernest-domain-security
source_filename: papernest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.papernest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 07:06:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: papernest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papernest/refs/heads/main/security/papernest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Subscription Management
- Energy
- Telecom
- Insurance
- Home Services
- Consumer
- France
---
