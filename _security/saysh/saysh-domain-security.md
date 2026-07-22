---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: saysh.com
  spf: true
hosts:
- cert_expires: Sep  2 08:21:31 2026 GMT
  host: saysh.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saysh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saysh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Saysh
provider_slug: saysh
slug: saysh-domain-security
source_filename: saysh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saysh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 08:21:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: saysh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saysh/refs/heads/main/security/saysh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Consumer
- Footwear
- Retail
- Ecommerce
- Apparel
- Direct to Consumer
- Shopify
---
