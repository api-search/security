---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: irishopendata.com
  spf: false
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: irishopendata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ireland MCP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ireland MCP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ireland MCP
provider_slug: irishopendata-com
slug: irishopendata-com-domain-security
source_filename: irishopendata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: irishopendata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: irishopendata.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/irishopendata-com/security/irishopendata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Public Data
- Ireland
- Open Source
- Free
---
