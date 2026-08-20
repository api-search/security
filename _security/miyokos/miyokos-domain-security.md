---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: miyokos.com
  spf: true
hosts:
- cert_expires: Aug 31 23:25:32 2026 GMT
  host: miyokos.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miyokos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Miyokos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Miyokos
provider_slug: miyokos
slug: miyokos-domain-security
source_filename: miyokos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miyokos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 23:25:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: miyokos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miyokos/refs/heads/main/security/miyokos-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Planetary Health
- Plant-Based
- Food and Beverage
- E-Commerce
- Shopify
- Agent Commerce
- UCP
---
