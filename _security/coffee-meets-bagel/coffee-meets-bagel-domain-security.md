---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coffeemeetsbagel.com
  spf: true
hosts:
- cert_expires: Sep 15 22:12:46 2026 GMT
  host: coffeemeetsbagel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coffee Meets Bagel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coffee Meets Bagel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Coffee Meets Bagel
provider_slug: coffee-meets-bagel
slug: coffee-meets-bagel-domain-security
source_filename: coffee-meets-bagel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coffeemeetsbagel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 22:12:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coffeemeetsbagel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coffee-meets-bagel/refs/heads/main/security/coffee-meets-bagel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Dating
- Dating App
- Social
- Relationships
- Mobile App
---
