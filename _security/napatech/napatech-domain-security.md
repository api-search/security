---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: napatech.com
  spf: true
hosts:
- cert_expires: Sep  6 23:45:50 2026 GMT
  host: www.napatech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Napatech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Napatech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Napatech
provider_slug: napatech
slug: napatech-domain-security
source_filename: napatech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.napatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:45:50 2026 GMT\n  hsts: false\ndomains:\n- domain: napatech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/napatech/refs/heads/main/security/napatech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Infra Devtools
- Networking
- SmartNIC
- FPGA
- Network Monitoring
- Cybersecurity
- Packet Capture
- Hardware SDK
---
