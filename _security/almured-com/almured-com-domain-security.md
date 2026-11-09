---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: almured.com
  spf: true
hosts:
- cert_expires: Jan 12 20:50:54 2027 GMT
  host: almured.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Almured Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Almured, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Almured
provider_slug: almured-com
slug: almured-com-domain-security
source_filename: almured-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: almured.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 20:50:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: almured.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/almured-com/security/almured-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- KnowledgeNetwork
- Open Source
- Decentralized
---
