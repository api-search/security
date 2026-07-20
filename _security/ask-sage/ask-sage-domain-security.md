---
api_specs:
- filename: ask-sage-server-openapi.json
  format: json
  label: Ask Sage Server API
  slug: ask-sage-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/openapi/ask-sage-server-openapi.json
- filename: ask-sage-user-openapi.json
  format: json
  label: Ask Sage User API
  slug: ask-sage-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/openapi/ask-sage-user-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asksage.ai
  spf: true
hosts:
- cert_expires: Aug 25 06:00:09 2026 GMT
  host: www.asksage.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ask Sage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ask Sage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ask Sage
provider_slug: ask-sage
slug: ask-sage-domain-security
source_filename: ask-sage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asksage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 06:00:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asksage.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ask-sage/refs/heads/main/security/ask-sage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Generative AI
- Large Language Models
- Government
- Defense
- Compliance
- FedRAMP
---
