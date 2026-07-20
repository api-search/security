---
api_specs:
- filename: fini-openapi.yml
  format: yaml
  label: Fini AI API
  slug: fini-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fini/refs/heads/main/openapi/fini-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: usefini.com
  spf: true
hosts:
- cert_expires: Sep 26 03:09:43 2026 GMT
  host: usefini.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:57:01 2026 GMT
  host: docs.usefini.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 07:17:32 2026 GMT
  host: api-prod.usefini.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fini, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Fini
provider_slug: fini
slug: fini-domain-security
source_filename: fini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usefini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:09:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.usefini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-prod.usefini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:17:32 2026 GMT\n  hsts: null\ndomains:\n- domain: usefini.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fini/refs/heads/main/security/fini-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Customer Support
- Customer Experience
- Knowledge Management
- Conversational AI
- Voice AI
- Helpdesk
- Regulated Industries
---
