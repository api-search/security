---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: geometer.io
  spf: true
hosts:
- cert_expires: Sep 19 22:14:55 2026 GMT
  host: geometer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geometer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geometer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Geometer
provider_slug: geometer
slug: geometer-domain-security
source_filename: geometer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geometer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:14:55 2026 GMT\n  hsts: false\ndomains:\n- domain: geometer.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geometer/refs/heads/main/security/geometer-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Incubator
- Accelerator
- Startup Studio
- Venture
- San Francisco
- Technology
---
