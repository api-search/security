---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: utribe.one
  spf: true
hosts:
- cert_expires: Dec 26 03:52:41 2026 GMT
  host: utribe.one
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Utribe One Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubuntu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ubuntu
provider_slug: utribe-one
slug: utribe-one-domain-security
source_filename: utribe-one-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utribe.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 03:52:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: utribe.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/utribe-one/security/utribe-one-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Gold-Backed Tokens
- Digital Payments
- Cryptocurrency Alternative
---
