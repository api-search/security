---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coolerheads.com
  spf: true
hosts:
- cert_expires: Sep  7 12:18:57 2026 GMT
  host: www.coolerheads.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cooler Heads Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cooler Heads, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cooler Heads
provider_slug: cooler-heads
slug: cooler-heads-domain-security
source_filename: cooler-heads-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coolerheads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:18:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: coolerheads.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooler-heads/refs/heads/main/security/cooler-heads-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Devices
- Health Care
- Oncology
- Scalp Cooling
- Patient Care
- MCP
---
