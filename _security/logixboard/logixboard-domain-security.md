---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: logixboard.com
  spf: true
hosts:
- cert_expires: Sep 15 08:38:22 2026 GMT
  host: www.logixboard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logixboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logixboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Logixboard
provider_slug: logixboard
slug: logixboard-domain-security
source_filename: logixboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logixboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:38:22 2026 GMT\n  hsts: false\ndomains:\n- domain: logixboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logixboard/refs/heads/main/security/logixboard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Freight Forwarding
- Transportation
- Shipment Visibility
- Customer Experience
- SaaS
---
