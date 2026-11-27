---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kadent.so
  spf: true
hosts:
- cert_expires: Jan 15 12:47:25 2027 GMT
  host: kadent.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kadent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kadent
provider_slug: kadent-so
slug: kadent-so-domain-security
source_filename: kadent-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadent.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 12:47:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kadent.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kadent-so/security/kadent-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Security
- Runtime Security
- MCP Gateway
- Policy Enforcement
- Audit Evidence
---
