---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gaspos.co
  spf: true
hosts:
- cert_expires: Sep 15 10:41:19 2026 GMT
  host: gaspos.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gas Pos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gas POS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gas POS
provider_slug: gas-pos
slug: gas-pos-domain-security
source_filename: gas-pos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gaspos.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:41:19 2026 GMT\n  hsts: null\ndomains:\n- domain: gaspos.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gas-pos/refs/heads/main/security/gas-pos-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Point of Sale
- Payments
- Fuel
- Convenience Store
- Truck Stop
- Retail
- EMV
- Hardware
---
