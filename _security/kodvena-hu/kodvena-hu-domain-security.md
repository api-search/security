---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kodvena.hu
  spf: true
hosts:
- cert_expires: Jan 17 21:30:53 2027 GMT
  host: kodvena.hu
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kódvéna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kódvéna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kódvéna
provider_slug: kodvena-hu
slug: kodvena-hu-domain-security
source_filename: kodvena-hu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kodvena.hu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:30:53 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kodvena.hu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kodvena-hu/security/kodvena-hu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Development
- AI Assistant
- Custom Software
- E-Commerce
- Hungary
---
