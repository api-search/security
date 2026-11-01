---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: carbikly.com
  spf: true
hosts:
- cert_expires: Dec  4 08:02:43 2026 GMT
  host: carbikly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbikly Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for carbikly-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: carbikly-com
provider_slug: carbikly-com
slug: carbikly-com-domain-security
source_filename: carbikly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbikly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 08:02:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carbikly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/carbikly-com/security/carbikly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Car Tax
- UK
- Finance
- Calculator
- Automotive
---
