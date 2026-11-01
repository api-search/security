---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mactechsolutionsllc.com
  spf: true
hosts:
- cert_expires: Dec  8 19:10:12 2026 GMT
  host: mactechsolutionsllc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mactechsolutionsllc Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mactechsolutionsllc-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mactechsolutionsllc-com
provider_slug: mactechsolutionsllc-com
slug: mactechsolutionsllc-com-domain-security
source_filename: mactechsolutionsllc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mactechsolutionsllc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 19:10:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mactechsolutionsllc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mactechsolutionsllc-com/security/mactechsolutionsllc-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- CMMC
- NIST-800-171
- DFARS
- SDVOSB
- Compliance
---
