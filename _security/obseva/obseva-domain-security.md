---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: obseva.com
  spf: false
hosts:
- cert_expires: Jan 13 13:30:57 2027 GMT
  host: www.obseva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Obseva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Obseva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Obseva
provider_slug: obseva
slug: obseva-domain-security
source_filename: obseva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.obseva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 13:30:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: obseva.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/obseva/security/obseva-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Monitoring
- Analytics
- AI
- Enterprise
---
