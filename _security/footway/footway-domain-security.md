---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: footway.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: footway.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.footway.co.uk
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 14:11:34 2026 GMT
  host: footway.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Footway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Footway, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Footway
provider_slug: footway
slug: footway-domain-security
source_filename: footway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.footway.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: footway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 14:11:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: footway.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: footway.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footway/refs/heads/main/security/footway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-commerce
- Marketplace
- Retail
- Footwear
- Fashion
- Shopify
- Agent Commerce
- UCP
- MCP
- Nordic
---
