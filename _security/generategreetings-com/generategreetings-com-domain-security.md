---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: generategreetings.com
  spf: true
hosts:
- cert_expires: Dec 19 15:03:52 2026 GMT
  host: generategreetings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Generate Greetings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generate Greetings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Generate Greetings
provider_slug: generategreetings-com
slug: generategreetings-com-domain-security
source_filename: generategreetings-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: generategreetings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 15:03:52 2026 GMT\n  hsts: false\ndomains:\n- domain: generategreetings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/generategreetings-com/security/generategreetings-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Greetings
- Personalization
- Cards
- Online
---
