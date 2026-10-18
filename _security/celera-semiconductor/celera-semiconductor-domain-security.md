---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: celerasemi.com
  spf: true
hosts:
- cert_expires: Feb 28 20:42:49 2027 GMT
  host: celerasemi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celera Semiconductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celera Semiconductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Celera Semiconductor
provider_slug: celera-semiconductor
slug: celera-semiconductor-domain-security
source_filename: celera-semiconductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celerasemi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 20:42:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: celerasemi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celera-semiconductor/refs/heads/main/security/celera-semiconductor-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Analog
- Artificial Intelligence
- Automation
---
