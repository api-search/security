---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datao.ma
  spf: true
hosts:
- cert_expires: Jan 17 17:49:48 2027 GMT
  host: datao.ma
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Datao
provider_slug: datao-ma
slug: datao-ma-domain-security
source_filename: datao-ma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datao.ma\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 17:49:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datao.ma\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/datao-ma/security/datao-ma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Procurement
- Morocco
- Public Data
- Software-as-a-Service
- Company
---
