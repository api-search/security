---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flycrates.com
  spf: false
hosts:
- cert_expires: Oct 13 01:07:20 2026 GMT
  host: flycrates.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flycrates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flycrates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Flycrates
provider_slug: flycrates
slug: flycrates-domain-security
source_filename: flycrates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flycrates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:07:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flycrates.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flycrates/refs/heads/main/security/flycrates-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Shipping
- Logistics
- International Shipping
- Cross-border eCommerce
- Amazon
- Package Forwarding
- Freight Forwarding
- Consumer
---
