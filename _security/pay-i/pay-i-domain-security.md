---
api_specs:
- filename: pay-i-openapi.yml
  format: yaml
  label: Pay-i API
  slug: pay-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/openapi/pay-i-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pay-i.com
  spf: true
hosts:
- cert_expires: Nov 18 02:58:10 2026 GMT
  host: www.pay-i.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 01:06:58 2026 GMT
  host: docs.pay-i.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 20:28:02 2026 GMT
  host: api.pay-i.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pay I Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pay-i, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pay-i
provider_slug: pay-i
slug: pay-i-domain-security
source_filename: pay-i-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pay-i.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 02:58:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pay-i.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 01:06:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pay-i.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 20:28:02 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: pay-i.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pay-i/refs/heads/main/security/pay-i-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- FinOps
- Observability
- Cost Management
- Generative AI
- LLM
- Analytics
- Governance
- Metering
---
