---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gbatteries.com
  spf: true
hosts:
- cert_expires: Sep 30 03:22:37 2026 GMT
  host: www.gbatteries.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gbatteries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gbatteries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gbatteries
provider_slug: gbatteries
slug: gbatteries-domain-security
source_filename: gbatteries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gbatteries.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 03:22:37 2026 GMT\n  hsts: false\ndomains:\n- domain: gbatteries.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gbatteries/refs/heads/main/security/gbatteries-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Batteries
- Energy Storage
- Electric Mobility
- Battery Management
- Fast Charging
- Lithium Metal
- Deeptech
- Hardware
---
