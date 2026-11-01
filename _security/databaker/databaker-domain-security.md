---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data-baker.ai
  spf: true
hosts:
- cert_expires: Dec 15 00:01:50 2026 GMT
  host: www.data-baker.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Databaker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databaker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Databaker
provider_slug: databaker
slug: databaker-domain-security
source_filename: databaker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data-baker.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 00:01:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: data-baker.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/databaker/security/databaker-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Artificial Intelligence
- Data Annotation
- Machine Learning
- Training Data
---
