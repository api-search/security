---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fizzl.eu
  spf: false
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: fizzl.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fizzl Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fizzl-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: fizzl-eu
provider_slug: fizzl-eu
slug: fizzl-eu-domain-security
source_filename: fizzl-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fizzl.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fizzl.eu\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fizzl-eu/security/fizzl-eu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Payments
- Automation
- Tools
- Platform
---
