---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: numertel.pl
  spf: true
hosts:
- cert_expires: Dec 26 07:22:03 2026 GMT
  host: numertel.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NumerTel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NumerTel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NumerTel
provider_slug: numertel-pl
slug: numertel-pl-domain-security
source_filename: numertel-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numertel.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 07:22:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numertel.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/numertel-pl/security/numertel-pl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Telecommunications
- Phone Lookup
- Spam Detection
- Poland
---
