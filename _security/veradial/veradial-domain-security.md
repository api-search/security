---
api_specs:
- filename: veradial-openapi-generated.yml
  format: yaml
  label: VeraDial Zapier Integration API
  slug: zapier-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/openapi/_ae-authored/veradial-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veradial.com
  spf: true
hosts:
- cert_expires: Dec 16 04:34:44 2026 GMT
  host: veradial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 08:52:01 2026 GMT
  host: api.veradial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Veradial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VeraDial, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VeraDial
provider_slug: veradial
slug: veradial-domain-security
source_filename: veradial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veradial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 04:34:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.veradial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 08:52:01 2026 GMT\n  hsts: false\ndomains:\n- domain: veradial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veradial/refs/heads/main/security/veradial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Receptionist
- Business Phone
- Telephony
- Voice AI
- SMS
- Webhook
- MCP
- Small Business
---
