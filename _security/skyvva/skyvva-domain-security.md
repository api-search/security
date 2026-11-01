---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: skyvva.com
  spf: false
hosts:
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: skyvva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skyvva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SKYVVA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SKYVVA
provider_slug: skyvva
slug: skyvva-domain-security
source_filename: skyvva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skyvva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: skyvva.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/skyvva/security/skyvva-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Integration
- Salesforce
- ERP
- Middleware-free
---
