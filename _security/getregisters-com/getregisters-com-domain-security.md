---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getregisters.com
  spf: true
hosts:
- cert_expires: Dec 24 12:04:14 2026 GMT
  host: getregisters.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Get Registers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get Registers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Get Registers
provider_slug: getregisters-com
slug: getregisters-com-domain-security
source_filename: getregisters-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getregisters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 12:04:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: getregisters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getregisters-com/security/getregisters-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Licensing
- Childcare
- Packaging
- Dental
- Home Care
---
