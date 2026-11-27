---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joules.cc
  spf: true
hosts:
- cert_expires: Jan 28 21:15:24 2027 GMT
  host: joules.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joules Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joules, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Joules
provider_slug: joules-cc
slug: joules-cc-domain-security
source_filename: joules-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joules.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 21:15:24 2027 GMT\n  hsts: false\ndomains:\n- domain: joules.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/joules-cc/security/joules-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Coaching
- Cycling
- ChatGPT
- Claude
---
