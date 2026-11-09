---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: argus.ing
  spf: true
hosts:
- cert_expires: Jan  9 00:58:00 2027 GMT
  host: argus.ing
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Argus Ing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Argus
provider_slug: argus-ing
slug: argus-ing-domain-security
source_filename: argus-ing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argus.ing\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 00:58:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: argus.ing\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/argus-ing/security/argus-ing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tender
- Procurement
- Analytics
- Artificial Intelligence
- Belgium
---
