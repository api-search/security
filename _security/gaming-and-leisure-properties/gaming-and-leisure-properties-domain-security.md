---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: glpropinc.com
  spf: true
hosts:
- cert_expires: Aug 10 10:08:08 2026 GMT
  host: www.glpropinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gaming And Leisure Properties Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gaming and Leisure Properties, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gaming and Leisure Properties
provider_slug: gaming-and-leisure-properties
slug: gaming-and-leisure-properties-domain-security
source_filename: gaming-and-leisure-properties-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glpropinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 10:08:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glpropinc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gaming-and-leisure-properties/refs/heads/main/security/gaming-and-leisure-properties-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Casinos
- Gaming
- Hospitality
- Real Estate
- REIT
- Triple-Net Lease
---
