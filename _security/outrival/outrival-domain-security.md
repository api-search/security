---
api_specs:
- filename: outrival-v1-openapi-original.json
  format: json
  label: OutRival API v1
  slug: outrival-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v1-openapi-original.json
- filename: outrival-v2-openapi-original.json
  format: json
  label: OutRival API v2
  slug: outrival-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/openapi/outrival-v2-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outrival.com
  spf: true
hosts:
- cert_expires: Sep 20 19:03:10 2026 GMT
  host: outrival.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.outrival.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outrival Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OutRival, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OutRival
provider_slug: outrival
slug: outrival-domain-security
source_filename: outrival-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outrival.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:03:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.outrival.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: outrival.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outrival/refs/heads/main/security/outrival-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Saas
- Conversational AI
- AI Agents
- Voice
- SMS
- Customer Engagement
- Chatbots
- Contact Center
- Webhooks
---
