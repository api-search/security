---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lightberry.com
  spf: true
hosts:
- cert_expires: Sep 16 17:26:14 2026 GMT
  host: lightberry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightberry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightberry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lightberry
provider_slug: lightberry
slug: lightberry-domain-security
source_filename: lightberry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightberry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:26:14 2026 GMT\n  hsts: false\ndomains:\n- domain: lightberry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightberry/refs/heads/main/security/lightberry-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Artificial Intelligence
- Conversational AI
- Voice
- Hardware
- Model Context Protocol
- Agents
- Y Combinator
---
