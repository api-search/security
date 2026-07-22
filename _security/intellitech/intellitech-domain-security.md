---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intellitech.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.intellitech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intellitech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intellitech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Intellitech
provider_slug: intellitech
slug: intellitech-domain-security
source_filename: intellitech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intellitech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: intellitech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intellitech/refs/heads/main/security/intellitech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductor Test
- JTAG
- Boundary Scan
- IEEE 1149.1
- Design for Test
- FPGA
- PCB Testing
- Embedded Systems
- Hardware
---
