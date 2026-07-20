---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomthis.co
  spf: true
hosts:
- cert_expires: Aug 27 17:18:02 2026 GMT
  host: bloomthis.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomthis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BloomThis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BloomThis
provider_slug: bloomthis
slug: bloomthis-domain-security
source_filename: bloomthis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bloomthis.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:18:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bloomthis.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomthis/refs/heads/main/security/bloomthis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Flowers
- Gifting
- Ecommerce
- Retail
- Shopify
- Agent Commerce
- MCP
- Malaysia
---
