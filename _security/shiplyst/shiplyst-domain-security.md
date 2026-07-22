---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shiplyst.com
  spf: true
hosts:
- cert_expires: Sep  1 06:03:57 2026 GMT
  host: shiplyst.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shiplyst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shiplyst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Shiplyst
provider_slug: shiplyst
slug: shiplyst-domain-security
source_filename: shiplyst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shiplyst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:03:57 2026 GMT\n  hsts: false\ndomains:\n- domain: shiplyst.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiplyst/refs/heads/main/security/shiplyst-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Shipping
- Ocean Freight
- Supply Chain
- Freight Forwarding
- Container Shipping
- Cargo Tracking
- Marketplace
---
