---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fmlane.com
  spf: true
hosts:
- cert_expires: Jan 31 16:30:02 2027 GMT
  host: fmlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fmlane Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FMlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FMlane
provider_slug: fmlane-com
slug: fmlane-com-domain-security
source_filename: fmlane-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fmlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 16:30:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fmlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fmlane-com/security/fmlane-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Facility Management
- Maintenance Software
- Condition Assessment
- Preventive Maintenance
- Asset Management
- Building Management
---
