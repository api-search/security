---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: renogy.com
  spf: true
hosts:
- cert_expires: Feb  3 04:11:51 2027 GMT
  host: renogy.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Renogy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Renogy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Renogy
provider_slug: renogy
slug: renogy-domain-security
source_filename: renogy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: renogy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 04:11:51 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: renogy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/renogy/security/renogy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Solar
- Renewable Energy
- Off-Grid
- Energy Solutions
---
