---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lottie.org
  spf: true
hosts:
- cert_expires: Aug 19 07:32:57 2026 GMT
  host: lottie.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lottie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lottie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lottie
provider_slug: lottie
slug: lottie-domain-security
source_filename: lottie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lottie.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lottie.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lottie/refs/heads/main/security/lottie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Care Homes
- Elderly Care
- Retirement Living
- Home Care
- Marketplace
- United Kingdom
---
