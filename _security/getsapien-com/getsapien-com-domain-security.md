---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getsapien.com
  spf: false
hosts:
- cert_expires: Dec  2 22:40:40 2026 GMT
  host: www.getsapien.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getsapien Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapien, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sapien
provider_slug: getsapien-com
slug: getsapien-com-domain-security
source_filename: getsapien-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getsapien.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 22:40:40 2026 GMT\n  hsts: null\ndomains:\n- domain: getsapien.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getsapien-com/security/getsapien-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Operations
- Analytics
- AI
- Manufacturing
- Retail
- Healthcare
---
