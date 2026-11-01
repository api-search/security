---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jacobs-university.de
  spf: true
hosts:
- cert_expires: Jan 12 17:34:28 2027 GMT
  host: www.jacobs-university.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constructor University Bremen Ggmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constructor University Bremen gGmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Constructor University Bremen gGmbH
provider_slug: constructor-university-bremen-ggmbh
slug: constructor-university-bremen-ggmbh-domain-security
source_filename: constructor-university-bremen-ggmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jacobs-university.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:34:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jacobs-university.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/constructor-university-bremen-ggmbh/security/constructor-university-bremen-ggmbh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Education
- Research
- University
- Germany
- Non-profit
- Company
---
