---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anthra.com
  spf: true
hosts:
- cert_expires: Jan  3 16:17:57 2027 GMT
  host: anthra.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anthra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anthra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anthra
provider_slug: anthra-com
slug: anthra-com-domain-security
source_filename: anthra-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anthra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:17:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: anthra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anthra-com/security/anthra-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- BookCreation
- Writing
- Illustration
- Audiobook
---
