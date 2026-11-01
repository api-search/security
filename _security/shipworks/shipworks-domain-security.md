---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shipworks.com
  spf: true
hosts:
- cert_expires: Jan 12 02:55:30 2027 GMT
  host: shipworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shipworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipWorks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShipWorks
provider_slug: shipworks
slug: shipworks-domain-security
source_filename: shipworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shipworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 02:55:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shipworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/shipworks/security/shipworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- E-commerce
- Logistics
- Software
- Integration
---
