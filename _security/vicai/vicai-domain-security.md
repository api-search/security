---
api_specs:
- filename: vicai-openapi-original.json
  format: json
  label: Vic.ai API
  slug: vicai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vicai/refs/heads/main/openapi/vicai-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vic.ai
  spf: true
hosts:
- cert_expires: Oct 12 22:13:05 2026 GMT
  host: www.vic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vicai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vic.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vic.ai
provider_slug: vicai
slug: vicai-domain-security
source_filename: vicai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:13:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vicai/refs/heads/main/security/vicai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounts Payable
- Invoicing
- Payments
- ERP Integration
- AI
- Finance Automation
- Webhooks
---
