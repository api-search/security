---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: resilientpower.com
  spf: true
hosts:
- cert_expires: Oct 11 16:20:48 2026 GMT
  host: resilientpower.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resilient Power Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resilient Power Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Resilient Power Systems
provider_slug: resilient-power-systems
slug: resilient-power-systems-domain-security
source_filename: resilient-power-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resilientpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:20:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: resilientpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resilient-power-systems/refs/heads/main/security/resilient-power-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Power Electronics
- Energy
- Hardware
- EV Charging
- Electrical Grid
- Manufacturing
---
