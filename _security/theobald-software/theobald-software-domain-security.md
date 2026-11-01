---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: theobald-software.com
  spf: true
hosts:
- cert_expires: Jan  4 17:00:03 2027 GMT
  host: theobald-software.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Theobald Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theobald Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Theobald Software
provider_slug: theobald-software
slug: theobald-software-domain-security
source_filename: theobald-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theobald-software.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 17:00:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: theobald-software.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/theobald-software/security/theobald-software-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Integration
- SAP
- Data
- API
---
