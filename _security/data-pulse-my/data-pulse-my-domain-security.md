---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data-pulse.my
  spf: false
hosts:
- cert_expires: Jan 21 23:57:46 2027 GMT
  host: data-pulse.my
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data Pulse My Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data-pulse-my, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: data-pulse-my
provider_slug: data-pulse-my
slug: data-pulse-my-domain-security
source_filename: data-pulse-my-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data-pulse.my\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:57:46 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: data-pulse.my\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/data-pulse-my/security/data-pulse-my-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data
- Public
- Malaysia
- Datasets
---
