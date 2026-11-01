---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: strut.so
  spf: true
hosts:
- cert_expires: Jan 19 05:49:11 2027 GMT
  host: strut.so
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Strut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Strut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Strut
provider_slug: strut
slug: strut-domain-security
source_filename: strut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: strut.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 05:49:11 2027 GMT\n  hsts: false\ndomains:\n- domain: strut.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/strut/security/strut-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Writing
- Workspace
- Notebook
- Long-form
---
