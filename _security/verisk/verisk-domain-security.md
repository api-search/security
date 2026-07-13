---
api_specs:
- filename: verisk-insurance-analytics-openapi.yml
  format: yaml
  label: Verisk Insurance Analytics API
  slug: insurance-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-insurance-analytics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verisk.com
  spf: true
hosts:
- cert_expires: Oct  7 00:29:31 2026 GMT
  host: www.verisk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: gateway-documentation.verisk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: gateway.verisk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verisk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verisk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verisk
provider_slug: verisk
slug: verisk-domain-security
source_filename: verisk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:29:31 2026 GMT\n  hsts: false\n- host: gateway-documentation.verisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: gateway.verisk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verisk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/security/verisk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Analytics
- Risk Management
- Property Data
- Catastrophe Modeling
- Underwriting
- Claims
---
