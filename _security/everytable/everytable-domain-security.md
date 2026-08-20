---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everytable.com
  spf: true
hosts:
- cert_expires: Sep 14 17:29:02 2026 GMT
  host: everytable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 02:56:37 2026 GMT
  host: account.everytable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everytable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everytable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Everytable
provider_slug: everytable
slug: everytable-domain-security
source_filename: everytable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everytable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:29:02 2026 GMT\n  hsts: null\n- host: account.everytable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:56:37 2026 GMT\n  hsts: null\ndomains:\n- domain: everytable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everytable/refs/heads/main/security/everytable-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food
- Restaurant
- Meal Delivery
- E-Commerce
- Agentic Commerce
- Shopify
- Social Enterprise
- Nutrition
- Subscription
---
