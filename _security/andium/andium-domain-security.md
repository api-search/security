---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: andium.com
  spf: true
hosts:
- cert_expires: Oct 18 07:42:28 2026 GMT
  host: www.andium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 05:57:34 2026 GMT
  host: shop.andium.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Andium
provider_slug: andium
slug: andium-domain-security
source_filename: andium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.andium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 07:42:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: shop.andium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:57:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: andium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andium/refs/heads/main/security/andium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Industrial IoT
- Remote Monitoring
- Methane Detection
- Emissions
- Computer Vision
- Edge Computing
- Commerce
- Model Context Protocol
---
