---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linuxfoundation.eu
  spf: true
hosts:
- cert_expires: Sep 28 12:43:40 2026 GMT
  host: linuxfoundation.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linux Foundation Europe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linux Foundation Europe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linux Foundation Europe
provider_slug: linux-foundation-europe
slug: linux-foundation-europe-domain-security
source_filename: linux-foundation-europe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linuxfoundation.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:43:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linuxfoundation.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linux-foundation-europe/refs/heads/main/security/linux-foundation-europe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Europe
- Governance
- Linux Foundation
- Open Source
---
