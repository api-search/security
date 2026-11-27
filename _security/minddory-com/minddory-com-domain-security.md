---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: minddory.com
  spf: true
hosts:
- cert_expires: Jan  4 14:46:26 2027 GMT
  host: minddory.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MindDory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MindDory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MindDory
provider_slug: minddory-com
slug: minddory-com-domain-security
source_filename: minddory-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minddory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:46:26 2027 GMT\n  hsts: false\ndomains:\n- domain: minddory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/minddory-com/security/minddory-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Language Learning
- Mobile App
- Vocabulary
- Artificial Intelligence
- Flashcards
---
