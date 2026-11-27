---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getsign.io
  spf: true
hosts:
- cert_expires: Dec 13 04:32:37 2026 GMT
  host: getsign.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GetSign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetSign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GetSign
provider_slug: getsign-io
slug: getsign-io-domain-security
source_filename: getsign-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsign.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 04:32:37 2026 GMT\n  hsts: false\ndomains:\n- domain: getsign.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getsign-io/security/getsign-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Document Management
- E-Signature
- Artificial Intelligence
- monday.com Integration
- Software-as-a-Service
---
