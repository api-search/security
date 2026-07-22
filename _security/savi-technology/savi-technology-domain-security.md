---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: savi.com
  spf: true
hosts:
- cert_expires: Aug 31 16:24:06 2026 GMT
  host: www.savi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savi Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savi Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Savi Technology
provider_slug: savi-technology
slug: savi-technology-domain-security
source_filename: savi-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.savi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:24:06 2026 GMT\n  hsts: false\ndomains:\n- domain: savi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savi-technology/refs/heads/main/security/savi-technology-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Supply Chain
- Logistics
- IoT
- RFID
- Asset Tracking
- Sensors
- Visibility
---
