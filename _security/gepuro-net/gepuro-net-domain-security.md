---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gepuro.net
  spf: true
hosts:
- cert_expires: Jan 14 21:48:34 2027 GMT
  host: gepuro.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gepuro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gepuro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gepuro
provider_slug: gepuro-net
slug: gepuro-net-domain-security
source_filename: gepuro-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gepuro.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 21:48:34 2027 GMT\n  hsts: false\ndomains:\n- domain: gepuro.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gepuro-net/security/gepuro-net-domain-security.yml
summary_line: TLSv1.3
tags:
- Data Science
- Machine Learning
- Consulting
- Python
- R
---
