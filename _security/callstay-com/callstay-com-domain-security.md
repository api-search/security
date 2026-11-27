---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: callstay.com
  spf: true
hosts:
- cert_expires: Jan  7 15:47:02 2027 GMT
  host: callstay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Callstay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callstay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Callstay
provider_slug: callstay-com
slug: callstay-com-domain-security
source_filename: callstay-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callstay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:47:02 2027 GMT\n  hsts: false\ndomains:\n- domain: callstay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/callstay-com/security/callstay-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Travel
- Hotels
- Hotel Booking
- Accommodation
- Reservations
- MCP
- AI Agents
---
