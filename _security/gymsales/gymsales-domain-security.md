---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gymsales.net
  spf: true
hosts:
- cert_expires: Jan 22 06:34:28 2027 GMT
  host: gymsales.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GymSales Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GymSales, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GymSales
provider_slug: gymsales
slug: gymsales-domain-security
source_filename: gymsales-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gymsales.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 06:34:28 2027 GMT\n  hsts: false\ndomains:\n- domain: gymsales.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gymsales/security/gymsales-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lead Management
- Sales Platform
- Club Management
- Performance Reporting
---
