---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeterlink.com
  spf: true
hosts:
- cert_expires: Oct 17 21:23:25 2026 GMT
  host: aeterlink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeterlinkcorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeterlink Corp., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aeterlink Corp.
provider_slug: aeterlinkcorp
slug: aeterlinkcorp-domain-security
source_filename: aeterlinkcorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aeterlink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:23:25 2026 GMT\n  hsts: false\ndomains:\n- domain: aeterlink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeterlinkcorp/refs/heads/main/security/aeterlinkcorp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Wireless Power
- IoT
- Hardware
- Industrial Automation
- Building Management
- Medical Devices
- Deep Tech
- Japan
---
