---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: color-chip.com
  spf: true
hosts:
- cert_expires: Dec  6 02:45:31 2026 GMT
  host: www.color-chip.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Colorchip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ColorChip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ColorChip
provider_slug: colorchip
slug: colorchip-domain-security
source_filename: colorchip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.color-chip.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 02:45:31 2026 GMT\n  hsts: false\ndomains:\n- domain: color-chip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/colorchip/refs/heads/main/security/colorchip-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Optical
- DataCenter
- Networking
- Hardware
---
