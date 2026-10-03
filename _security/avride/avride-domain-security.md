---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avride.ai
  spf: true
hosts:
- cert_expires: Nov 10 00:42:45 2026 GMT
  host: www.avride.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avride Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avride, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Avride
provider_slug: avride
slug: avride-domain-security
source_filename: avride-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avride.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 00:42:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avride.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avride/refs/heads/main/security/avride-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Autonomous Vehicles
- Delivery Robots
- Artificial Intelligence
- Mobility
- Technology
---
