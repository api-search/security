---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: restcase.com
  spf: false
hosts:
- cert_expires: Jan 16 11:56:40 2027 GMT
  host: restcase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Restcase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guy Levin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Guy Levin
provider_slug: restcase
slug: restcase-domain-security
source_filename: restcase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restcase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 11:56:40 2027 GMT\n  hsts: false\ndomains:\n- domain: restcase.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/restcase/security/restcase-domain-security.yml
summary_line: TLSv1.3
tags:
- API Development
- Design-First
- Collaboration
- Productivity
- Platform
- Company
---
