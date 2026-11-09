---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dadev.nl
  spf: true
hosts:
- cert_expires: Feb  2 18:02:44 2027 GMT
  host: dadev.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dadev Nl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Do App Dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Do App Dev
provider_slug: dadev-nl
slug: dadev-nl-domain-security
source_filename: dadev-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dadev.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 18:02:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dadev.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dadev-nl/security/dadev-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software Development
- Automation
- B2B Solutions
- Integration
---
