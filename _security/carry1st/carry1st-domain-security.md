---
api_specs:
- filename: carry1st-pay1st-gateway-openapi.yml
  format: yaml
  label: Pay1st Gateway API
  slug: pay1st-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/openapi/carry1st-pay1st-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: carry1st.com
  spf: true
hosts:
- cert_expires: Oct  1 14:26:15 2026 GMT
  host: www.carry1st.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 10:50:08 2026 GMT
  host: pay1st-docs.carry1st.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api-gateway.carry1st.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carry1St Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carry1st, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Carry1st
provider_slug: carry1st
slug: carry1st-domain-security
source_filename: carry1st-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carry1st.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:26:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pay1st-docs.carry1st.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-gateway.carry1st.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: carry1st.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carry1st/refs/heads/main/security/carry1st-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Gateway
- Fintech
- Gaming
- Mobile Games
- Africa
- Digital Commerce
- Merchant of Record
- Games Publishing
---
