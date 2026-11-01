---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getdashdot.com
  spf: false
hosts:
- cert_expires: Jan 22 11:41:54 2027 GMT
  host: getdashdot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dashdot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dash., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dash.
provider_slug: dashdot
slug: dashdot-domain-security
source_filename: dashdot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getdashdot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:41:54 2027 GMT\n  hsts: false\ndomains:\n- domain: getdashdot.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dashdot/security/dashdot-domain-security.yml
summary_line: TLSv1.3
tags:
- Monitoring
- OpenSource
- Dashboard
- Server
- SingleNode
- Docker
---
