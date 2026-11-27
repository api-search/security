---
api_specs:
- filename: conveo-ai-interviews-api-openapi.yml
  format: yaml
  label: Conveo Interviews API
  slug: conveo-ai-interviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveo-ai/openapi/conveo-ai-interviews-api-openapi.yml
- filename: conveo-ai-studies-api-openapi.yml
  format: yaml
  label: Conveo Studies API
  slug: conveo-ai-studies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/conveo-ai/openapi/conveo-ai-studies-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conveo.ai
  spf: true
hosts:
- cert_expires: Jan  3 20:46:09 2027 GMT
  host: conveo.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conveo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conveo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conveo
provider_slug: conveo-ai
slug: conveo-ai-domain-security
source_filename: conveo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conveo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:46:09 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: conveo.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/conveo-ai/security/conveo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Qualitative Research
- Market Research
- Customer Interviews
- Consumer Insights
- MCP
---
