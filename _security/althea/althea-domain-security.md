---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: althea.kr
  spf: true
hosts:
- cert_expires: Aug 29 15:44:02 2026 GMT
  host: us.althea.kr
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Althea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Althea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Althea
provider_slug: althea
slug: althea-domain-security
source_filename: althea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.althea.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:44:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: althea.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/althea/refs/heads/main/security/althea-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- Retail
- Beauty
- Cosmetics
- K-Beauty
- Skincare
- Agent Commerce
- Shopify
---
