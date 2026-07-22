---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tsmc.com
  spf: true
hosts:
- cert_expires: Sep 30 17:59:20 2026 GMT
  host: www.tsmc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TSMC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TSMC
provider_slug: tsmc
slug: tsmc-domain-security
source_filename: tsmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsmc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tsmc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsmc/refs/heads/main/security/tsmc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Semiconductors
- Technology
- Manufacturing
---
