---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gamerspilot.com
  spf: true
hosts:
- cert_expires: Feb  4 23:45:45 2027 GMT
  host: gamerspilot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GamersPilot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GamersPilot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GamersPilot
provider_slug: gamerspilot-com
slug: gamerspilot-com-domain-security
source_filename: gamerspilot-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gamerspilot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:45:45 2027 GMT\n  hsts: false\ndomains:\n- domain: gamerspilot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gamerspilot-com/security/gamerspilot-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Gaming
- Steam
- Backlog
- Planner
- Tools
---
