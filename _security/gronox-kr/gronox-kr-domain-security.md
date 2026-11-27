---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gronox.kr
  spf: true
hosts:
- cert_expires: Jan  4 01:42:33 2027 GMT
  host: gronox.kr
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GRONOX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GRONOX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GRONOX
provider_slug: gronox-kr
slug: gronox-kr-domain-security
source_filename: gronox-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gronox.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:42:33 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: gronox.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gronox-kr/security/gronox-kr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Quantum-Safe
- Data Integration
- Enterprise
- Security
---
