---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trymason.com
  spf: false
hosts:
- cert_expires: Jan 15 15:23:52 2027 GMT
  host: www.trymason.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trymason Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mason
provider_slug: trymason-com
slug: trymason-com-domain-security
source_filename: trymason-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trymason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 15:23:52 2027 GMT\n  hsts: false\ndomains:\n- domain: trymason.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/trymason-com/security/trymason-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API
- Integration
- Automation
- Platform
---
