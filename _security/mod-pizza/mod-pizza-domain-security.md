---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modpizza.com
  spf: true
hosts:
- cert_expires: Nov 13 19:39:56 2026 GMT
  host: modpizza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mod Pizza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOD Pizza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MOD Pizza
provider_slug: mod-pizza
slug: mod-pizza-domain-security
source_filename: mod-pizza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modpizza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 19:39:56 2026 GMT\n  hsts: false\ndomains:\n- domain: modpizza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mod-pizza/refs/heads/main/security/mod-pizza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurant
- Food and Beverage
- Fast Casual
- Pizza
- Retail
- Consumer
- Loyalty
- Online Ordering
- Franchising
---
