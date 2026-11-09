---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: claidex.com
  spf: true
hosts:
- cert_expires: Dec 13 03:57:27 2026 GMT
  host: claidex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Claidex Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claidex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Claidex
provider_slug: claidex-com
slug: claidex-com-domain-security
source_filename: claidex-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claidex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 03:57:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claidex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/claidex-com/security/claidex-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biomedicine
- Clinical Trials
- Drug Discovery
- Research
---
