---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aioq.org
  spf: true
hosts:
- cert_expires: Jan  6 05:36:55 2027 GMT
  host: aioq.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aioq Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AIO
provider_slug: aioq-org
slug: aioq-org-domain-security
source_filename: aioq-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aioq.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 05:36:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: aioq.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aioq-org/security/aioq-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Integrity
- Open Standard
- Measurements
- Legal Reference Data
- Framework
- Research
- Regulations
---
