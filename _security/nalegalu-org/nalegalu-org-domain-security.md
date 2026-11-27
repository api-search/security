---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nalegalu.org
  spf: true
hosts:
- cert_expires: Feb  7 05:16:20 2027 GMT
  host: nalegalu.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nalegalu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nalegalu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nalegalu
provider_slug: nalegalu-org
slug: nalegalu-org-domain-security
source_filename: nalegalu-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nalegalu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 05:16:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: nalegalu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nalegalu-org/security/nalegalu-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Legal Tech
- Open Data
- Artificial Intelligence
- Poland
- Public Domain
---
