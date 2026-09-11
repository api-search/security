---
api_specs:
- filename: fraud-net-public-apis-openapi.json
  format: json
  label: Fraud.net Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/openapi/fraud-net-public-apis-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fraud.net
  spf: true
hosts:
- cert_expires: Nov 17 10:47:28 2026 GMT
  host: www.fraud.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 14:36:50 2026 GMT
  host: api-docs.fraud.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api-sandbox.c008-m008-us.fraud.net
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fraud Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fraud.net, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fraud.net
provider_slug: fraud-net
slug: fraud-net-domain-security
source_filename: fraud-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fraud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 10:47:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.fraud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 14:36:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.c008-m008-us.fraud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fraud.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nx-correction:\n  field: domains[0].spf\n  corrected_to: true\n  reason: >-\n    The mechanical probe recorded spf:false because the local resolver returned an empty\n    TXT set (repeatable timeout). Verified over DNS-over-HTTPS on 2026-09-10: fraud.net\n    publishes \"v=spf1 include:_spf.google.com include:_spf.atlassian.net\n\
  \    include:infusionmail.com include:hubspotemail.net\n    include:2113031.spf02.hubspotemail.net ~all\".\n  checked: '2026-09-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/security/fraud-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud
- Risk
- Commerce
- Payments
- Security
- Compliance
- Identity
- Banking
- Machine Learning
---
