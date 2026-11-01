---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mcpgatepro.com
  spf: true
hosts:
- cert_expires: Jan 13 08:50:39 2027 GMT
  host: mcpgatepro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcpgatepro Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcpgatepro-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mcpgatepro-com
provider_slug: mcpgatepro-com
slug: mcpgatepro-com-domain-security
source_filename: mcpgatepro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpgatepro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 08:50:39 2027 GMT\n  hsts: null\ndomains:\n- domain: mcpgatepro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mcpgatepro-com/security/mcpgatepro-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Cloud
- Cost-Management
- Database
- Monitoring
---
