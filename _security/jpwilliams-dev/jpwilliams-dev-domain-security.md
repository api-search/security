---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: jpwilliams.dev
  spf: true
hosts:
- cert_expires: Dec 17 22:18:43 2026 GMT
  host: jpwilliams.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jack Williams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jack Williams, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Jack Williams
provider_slug: jpwilliams-dev
slug: jpwilliams-dev-domain-security
source_filename: jpwilliams-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jpwilliams.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 22:18:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jpwilliams.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jpwilliams-dev/security/jpwilliams-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Software
- Developers
- Node.js
- React
- Open Source
---
