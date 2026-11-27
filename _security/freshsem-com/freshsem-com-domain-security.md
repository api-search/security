---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshsem.com
  spf: true
hosts:
- cert_expires: Jan 14 19:00:54 2027 GMT
  host: freshsem.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fresh SEM Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fresh SEM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fresh SEM
provider_slug: freshsem-com
slug: freshsem-com-domain-security
source_filename: freshsem-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freshsem.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 19:00:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshsem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freshsem-com/security/freshsem-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Marketing
- Lead Generation
- Digital Marketing
- SEO
- PPC
---
