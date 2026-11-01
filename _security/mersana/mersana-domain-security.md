---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mersana.com
  spf: true
hosts:
- cert_expires: Jan 14 05:24:14 2027 GMT
  host: www.mersana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mersana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mersana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mersana
provider_slug: mersana
slug: mersana-domain-security
source_filename: mersana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mersana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 05:24:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mersana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mersana/security/mersana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Oncology
- Therapeutics
- ClinicalTrials
- Company
---
