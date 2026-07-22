---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hellofresh.com
  spf: true
hosts:
- cert_expires: Oct  8 13:25:42 2026 GMT
  host: www.hellofresh.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hellofresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HelloFresh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HelloFresh
provider_slug: hellofresh
slug: hellofresh-domain-security
source_filename: hellofresh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hellofresh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:25:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hellofresh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hellofresh/refs/heads/main/security/hellofresh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Food and Beverage
- Meal Kit
- E-Commerce
- Subscription
- Open Source
- Retail
---
