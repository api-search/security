---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cropconex.com
  spf: true
hosts:
- cert_expires: Jan  4 02:27:16 2027 GMT
  host: cropconex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cropconex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CropConex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CropConex
provider_slug: cropconex
slug: cropconex-domain-security
source_filename: cropconex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cropconex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:27:16 2027 GMT\n  hsts: false\ndomains:\n- domain: cropconex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cropconex/refs/heads/main/security/cropconex-domain-security.yml
summary_line: TLSv1.3
tags:
- Agriculture
- SupplyChain
- CommodityManagement
- SaaS
- Platform
---
