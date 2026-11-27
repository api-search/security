---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcpcalc.com
  spf: false
hosts:
- cert_expires: Dec 31 19:45:39 2026 GMT
  host: mcpcalc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPCalc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPCalc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MCPCalc
provider_slug: mcpcalc-com
slug: mcpcalc-com-domain-security
source_filename: mcpcalc-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpcalc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:45:39 2026 GMT\n  hsts: false\ndomains:\n- domain: mcpcalc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcpcalc-com/security/mcpcalc-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Math
- Collaboration
- Calculator
- Workspace
- Education
---
