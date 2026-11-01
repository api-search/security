---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dozeehealth.ai
  spf: false
hosts:
- cert_expires: Nov 24 15:57:51 2026 GMT
  host: www.dozeehealth.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dozee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dozee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dozee
provider_slug: dozee
slug: dozee-domain-security
source_filename: dozee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dozeehealth.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 15:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dozeehealth.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dozee/security/dozee-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Remote Monitoring
- AI
- Ballistocardiography
---
