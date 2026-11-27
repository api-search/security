---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flightclaw.com
  spf: true
hosts:
- cert_expires: Jan  2 11:34:13 2027 GMT
  host: flightclaw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: flightclaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for flightclaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: flightclaw
provider_slug: flightclaw-com
slug: flightclaw-com-domain-security
source_filename: flightclaw-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flightclaw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:34:13 2027 GMT\n  hsts: false\ndomains:\n- domain: flightclaw.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flightclaw-com/security/flightclaw-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Flight Booking
- AI Agents
- MCP
- Travel
---
