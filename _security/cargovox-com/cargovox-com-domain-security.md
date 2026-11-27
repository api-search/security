---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: cargovox.com
  spf: true
hosts:
- cert_expires: Dec 13 20:33:23 2026 GMT
  host: cargovox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coservices OU Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coservices OU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Coservices OU
provider_slug: cargovox-com
slug: cargovox-com-domain-security
source_filename: cargovox-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cargovox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 20:33:23 2026 GMT\n  hsts: false\ndomains:\n- domain: cargovox.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cargovox-com/security/cargovox-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- AI Phone Agent
- Transport
- Logistics
- Moving Services
- CRM Integration
- Lead Capture
---
