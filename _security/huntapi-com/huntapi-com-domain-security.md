---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: huntapi.com
  spf: false
hosts:
- cert_expires: Dec 16 03:34:50 2026 GMT
  host: www.huntapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HuntAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HuntAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: HuntAPI
provider_slug: huntapi-com
slug: huntapi-com-domain-security
source_filename: huntapi-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huntapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 03:34:50 2026 GMT\n  hsts: false\ndomains:\n- domain: huntapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/huntapi-com/security/huntapi-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Video API
- Content Aggregation
- AI Training
- Social Media Monitoring
- Digital Signage
- Security Surveillance
- Advertising Intelligence
---
