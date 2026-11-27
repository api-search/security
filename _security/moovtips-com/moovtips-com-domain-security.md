---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moovtips.com
  spf: true
hosts:
- cert_expires: Dec 29 17:33:48 2026 GMT
  host: moovtips.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moovtips Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moovtips, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Moovtips
provider_slug: moovtips-com
slug: moovtips-com-domain-security
source_filename: moovtips-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moovtips.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: moovtips.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/moovtips-com/security/moovtips-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Agency
- Web Development
- AI Services
- SEO
- E-Commerce
- Small Business
---
