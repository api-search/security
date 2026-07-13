---
api_specs:
- filename: public_api.html
  format: yaml
  label: Paigo API
  slug: paigo-api
  spec_type: OpenAPI
  url: https://paigo-public-information.s3.us-east-2.amazonaws.com/public_api.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paigo.tech
  spf: true
hosts:
- host: www.paigo.tech
  https: false
- cert_expires: Sep 16 13:17:00 2026 GMT
  host: docs.paigo.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.prod.paigo.tech
  https: false
kind: domain-security
layout: security
method: probed
name: Paigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paigo, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paigo
provider_slug: paigo
slug: paigo-domain-security
source_filename: paigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paigo.tech\n  https: false\n- host: docs.paigo.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prod.paigo.tech\n  https: false\ndomains:\n- domain: paigo.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paigo/refs/heads/main/security/paigo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Usage-Based Billing
- Metering
- Invoicing
- Pricing
- SaaS
- Subscriptions
- Developer Tools
- FinOps
---
