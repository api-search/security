---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aiqbee.com
  spf: true
hosts:
- cert_expires: Jan 28 15:56:31 2027 GMT
  host: aiqbee.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiqbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aiqbee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aiqbee
provider_slug: aiqbee-com
slug: aiqbee-com-domain-security
source_filename: aiqbee-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiqbee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 15:56:31 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: aiqbee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aiqbee-com/security/aiqbee-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Memory
- Enterprise Knowledge
- LLM Governance
- Teams Integration
- Developer Tools
- AI Marketplace
---
