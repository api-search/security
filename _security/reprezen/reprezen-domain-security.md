---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reprezen.com
  spf: true
hosts:
- cert_expires: Dec 26 15:18:09 2026 GMT
  host: reprezen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reprezen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RepreZen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RepreZen
provider_slug: reprezen
slug: reprezen-domain-security
source_filename: reprezen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reprezen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:18:09 2026 GMT\n  hsts: null\ndomains:\n- domain: reprezen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/reprezen/security/reprezen-domain-security.yml
summary_line: TLSv1.3
tags:
- API Design
- Enterprise Software
- Modeling
- Integration
- Company
---
