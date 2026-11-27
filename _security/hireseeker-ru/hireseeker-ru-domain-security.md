---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hireseeker.ru
  spf: true
hosts:
- cert_expires: Jan 15 20:22:47 2027 GMT
  host: hireseeker.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HireSeeker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HireSeeker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HireSeeker
provider_slug: hireseeker-ru
slug: hireseeker-ru-domain-security
source_filename: hireseeker-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hireseeker.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 20:22:47 2027 GMT\n  hsts: false\ndomains:\n- domain: hireseeker.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hireseeker-ru/security/hireseeker-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IT
- Job
- Aggregator
- Artificial Intelligence
---
