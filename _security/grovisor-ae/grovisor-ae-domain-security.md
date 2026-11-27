---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: grovisor.ae
  spf: true
hosts:
- cert_expires: Dec 26 12:05:46 2026 GMT
  host: grovisor.ae
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grovisor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grovisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Grovisor
provider_slug: grovisor-ae
slug: grovisor-ae-domain-security
source_filename: grovisor-ae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grovisor.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:05:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: grovisor.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/grovisor-ae/security/grovisor-ae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Tax
- Accounting
- Business-Setup
- United Arab Emirates
---
