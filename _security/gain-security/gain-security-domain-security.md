---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gain.security
  spf: true
hosts:
- cert_expires: Jan 13 07:35:56 2027 GMT
  host: gain.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gain Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gain Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gain Security
provider_slug: gain-security
slug: gain-security-domain-security
source_filename: gain-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gain.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 07:35:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gain.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gain-security/security/gain-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Platform
- Threat-Detection
- Vulnerability-Management
---
