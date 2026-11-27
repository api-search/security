---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ihateinvoicing.io
  spf: false
hosts:
- cert_expires: Jan 12 13:53:25 2027 GMT
  host: ihateinvoicing.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: I Hate Invoicing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for I Hate Invoicing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: I Hate Invoicing
provider_slug: ihateinvoicing-io
slug: ihateinvoicing-io-domain-security
source_filename: ihateinvoicing-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ihateinvoicing.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:53:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ihateinvoicing.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ihateinvoicing-io/security/ihateinvoicing-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Invoicing
- Artificial Intelligence
- Freelance
- Software-as-a-Service
- Payments
- Company
---
