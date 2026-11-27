---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: millstead.io
  spf: true
hosts:
- cert_expires: Jan 31 17:02:33 2027 GMT
  host: millstead.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Millstead Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Millstead, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Millstead
provider_slug: millstead-io
slug: millstead-io-domain-security
source_filename: millstead-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: millstead.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 17:02:33 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: millstead.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/millstead-io/security/millstead-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Small Business
- No-Code
- Software-as-a-Service
- Automation
---
