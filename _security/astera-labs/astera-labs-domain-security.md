---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asteralabs.com
  spf: true
hosts:
- cert_expires: Oct 16 17:23:07 2026 GMT
  host: www.asteralabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astera Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astera Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Astera Labs
provider_slug: astera-labs
slug: astera-labs-domain-security
source_filename: astera-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asteralabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:23:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: asteralabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astera-labs/refs/heads/main/security/astera-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Semiconductors
- Hardware
- AI Infrastructure
- Data-Center
- Connectivity
- PCIe
- CXL
- Ethernet
- Fleet Management
- Telemetry
- Device Management
---
