---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: softwarehelden.com
  spf: true
hosts:
- cert_expires: Nov 29 11:35:39 2026 GMT
  host: softwarehelden.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Softwarehelden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Softwarehelden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Softwarehelden
provider_slug: softwarehelden
slug: softwarehelden-domain-security
source_filename: softwarehelden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: softwarehelden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 11:35:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: softwarehelden.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/softwarehelden/security/softwarehelden-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Digital Transformation
- Automation
- AutomotiveTesting
---
