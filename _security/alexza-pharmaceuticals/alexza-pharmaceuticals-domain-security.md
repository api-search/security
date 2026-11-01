---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alexza.com
  spf: true
hosts:
- cert_expires: Dec 31 04:36:56 2026 GMT
  host: www.alexza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alexza Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alexza Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alexza Pharmaceuticals
provider_slug: alexza-pharmaceuticals
slug: alexza-pharmaceuticals-domain-security
source_filename: alexza-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alexza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 04:36:56 2026 GMT\n  hsts: false\ndomains:\n- domain: alexza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/alexza-pharmaceuticals/security/alexza-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharma
- InhaledTherapies
- Rebranding
- Technology
---
