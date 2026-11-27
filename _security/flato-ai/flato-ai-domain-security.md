---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: flato.ai
  spf: true
hosts:
- cert_expires: Feb  4 08:11:09 2027 GMT
  host: flato.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flato.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flato.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Flato.ai
provider_slug: flato-ai
slug: flato-ai-domain-security
source_filename: flato-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flato.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 08:11:09 2027 GMT\n  hsts: false\ndomains:\n- domain: flato.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/flato-ai/security/flato-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Presentation
- Canvas
- Design
- MCP
---
