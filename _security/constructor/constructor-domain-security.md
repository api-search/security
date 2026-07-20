---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: constructor.com
  spf: true
hosts:
- cert_expires: Sep 18 08:47:56 2026 GMT
  host: constructor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Constructor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constructor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Constructor
provider_slug: constructor
slug: constructor-domain-security
source_filename: constructor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constructor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: constructor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/constructor/refs/heads/main/security/constructor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ecommerce
- Search
- Product Discovery
- Recommendations
- Personalization
- Retail
- AI
---
