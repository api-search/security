---
api_specs:
- filename: insightera-nlp-platform-openapi.yml
  format: yaml
  label: InsightEra NLP Platform API
  slug: insightera-nlp-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insightera/refs/heads/main/openapi/insightera-nlp-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insightera.co.th
  spf: true
hosts:
- cert_expires: Oct 28 16:35:22 2026 GMT
  host: www.insightera.co.th
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 00:10:04 2026 GMT
  host: nlp.insightera.co.th
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insightera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InsightEra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InsightEra
provider_slug: insightera
slug: insightera-domain-security
source_filename: insightera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insightera.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:35:22 2026 GMT\n  hsts: false\n- host: nlp.insightera.co.th\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 00:10:04 2026 GMT\n  hsts: null\ndomains:\n- domain: insightera.co.th\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insightera/refs/heads/main/security/insightera-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing Technology
- Social Listening
- Data Analytics
- Customer Data Platform
- CRM
- Chatbot
- Social Media Management
- Natural Language Processing
- Artificial Intelligence
---
