---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: homeschooltools.net
  spf: true
hosts:
- cert_expires: Feb  2 13:15:34 2027 GMT
  host: homeschooltools.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homeschool Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homeschool Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Homeschool Tools
provider_slug: homeschooltools-net
slug: homeschooltools-net-domain-security
source_filename: homeschooltools-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homeschooltools.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 13:15:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: homeschooltools.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/homeschooltools-net/security/homeschooltools-net-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Education
- Homeschool
- Curriculum
- Artificial Intelligence
- Resources
---
