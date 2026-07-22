---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wheelocity.com
  spf: true
hosts:
- cert_expires: Oct 12 02:17:39 2026 GMT
  host: www.wheelocity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wheelocity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wheelocity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Wheelocity
provider_slug: wheelocity
slug: wheelocity-domain-security
source_filename: wheelocity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wheelocity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 02:17:39 2026 GMT\n  hsts: false\ndomains:\n- domain: wheelocity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wheelocity/refs/heads/main/security/wheelocity-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Logistics
- Supply Chain
- Agriculture
- Grocery Delivery
- Rural Commerce
- Cold Chain
- Electric Vehicles
- India
---
