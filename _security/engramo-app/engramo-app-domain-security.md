---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: engramo.app
  spf: true
hosts:
- cert_expires: Feb  4 10:42:41 2027 GMT
  host: engramo.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EngrAmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EngrAmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EngrAmo
provider_slug: engramo-app
slug: engramo-app-domain-security
source_filename: engramo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engramo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 10:42:41 2027 GMT\n  hsts: false\ndomains:\n- domain: engramo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/engramo-app/security/engramo-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Language Learning
- Artificial Intelligence
- Education
- Flashcards
- Mobile App
---
