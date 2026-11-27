---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gsc-em.com
  spf: true
hosts:
- cert_expires: Dec 22 14:30:02 2026 GMT
  host: gsc-em.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: gsc-em-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gsc-em-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: gsc-em-com
provider_slug: gsc-em-com
slug: gsc-em-com-domain-security
source_filename: gsc-em-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gsc-em.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 14:30:02 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: gsc-em.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gsc-em-com/security/gsc-em-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Barcodes
- Artificial Intelligence
- Shopping
- Commerce
- Retail
- GTIN
---
