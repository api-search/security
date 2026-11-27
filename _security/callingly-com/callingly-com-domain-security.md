---
api_specs:
- filename: callingly-com-openapi-generated.yml
  format: yaml
  label: Callingly API
  slug: callingly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callingly-com/openapi/_ae-authored/callingly-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: callingly.com
  spf: true
hosts:
- cert_expires: Jan 29 17:32:33 2027 GMT
  host: callingly.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Callingly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callingly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Callingly
provider_slug: callingly-com
slug: callingly-com-domain-security
source_filename: callingly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callingly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 17:32:33 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: callingly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/callingly-com/security/callingly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Sales
- Lead Response
- Speed To Lead
- Telephony
- SMS
- AI Voice Agents
- MCP
---
