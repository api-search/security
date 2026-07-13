---
api_specs:
- filename: allianz-trade-payment-overdues.yaml
  format: yaml
  label: Allianz Trade Payment Overdues API
  slug: payment-overdues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-payment-overdues.yaml
- filename: allianz-trade-company-grade.yaml
  format: yaml
  label: Allianz Trade Company Grade API
  slug: company-grade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-company-grade.yaml
- filename: allianz-trade-claims.yaml
  format: yaml
  label: Allianz Trade Claims API
  slug: claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-claims.yaml
- filename: allianz-trade-policy.yaml
  format: yaml
  label: Allianz Trade Policy API
  slug: policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/openapi/allianz-trade-policy.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: allianz-trade.com
  spf: true
hosts:
- cert_expires: Oct  4 22:27:44 2026 GMT
  host: www.allianz-trade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 05:28:28 2026 GMT
  host: developers.allianz-trade.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.allianz-trade.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allianz Trade Online Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allianz Trade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allianz Trade
provider_slug: allianz-trade-online
slug: allianz-trade-online-domain-security
source_filename: allianz-trade-online-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allianz-trade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:27:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.allianz-trade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:28:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.allianz-trade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: allianz-trade.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allianz-trade-online/refs/heads/main/security/allianz-trade-online-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Credit Insurance
- Insurance
- Risk Management
- Trade Credit
- E-Commerce
- Surety
---
