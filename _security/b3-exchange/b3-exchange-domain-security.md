---
api_specs:
- filename: b3-exchange-investor-position-openapi.json
  format: json
  label: B3 Investor Area (Área do Investidor) APIs
  slug: b3-investor-area-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-investor-position-openapi.json
- filename: b3-exchange-tesouro-direto-bonds-openapi.json
  format: json
  label: B3 Tesouro Direto APIs
  slug: b3-tesouro-direto-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-tesouro-direto-bonds-openapi.json
- filename: b3-exchange-otc-public-info-openapi.json
  format: json
  label: B3 OTC (Balcão) APIs
  slug: b3-otc-balcao-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-otc-public-info-openapi.json
- filename: b3-exchange-core-calculation-openapi.json
  format: json
  label: B3 Listed Markets (Listados) APIs
  slug: b3-listed-markets-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-core-calculation-openapi.json
- filename: b3-exchange-isin-openapi.json
  format: json
  label: B3 ISIN API
  slug: b3-isin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-isin-openapi.json
- filename: b3-exchange-banco-b3-custody-openapi.json
  format: json
  label: Banco B3 APIs
  slug: b3-banco-b3-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-banco-b3-custody-openapi.json
- filename: b3-exchange-insurance-claim-openapi.json
  format: json
  label: B3 Insurance (Seguros) APIs
  slug: b3-insurance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-insurance-claim-openapi.json
- filename: b3-exchange-auth-client-credentials-openapi.json
  format: json
  label: B3 Authentication APIs
  slug: b3-authentication-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/openapi/b3-exchange-auth-client-credentials-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: b3.com.br
  spf: true
hosts:
- cert_expires: Sep  9 03:07:28 2026 GMT
  host: www.b3.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 03:07:28 2026 GMT
  host: developers.b3.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: B3 Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for B3 (Brasil Bolsa Balcão), probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: B3 (Brasil Bolsa Balcão)
provider_slug: b3-exchange
slug: b3-exchange-domain-security
source_filename: b3-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.b3.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:07:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.b3.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:07:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: b3.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/b3-exchange/refs/heads/main/security/b3-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial
- Market Data
- Stocks
- Trading
- Exchange
- Derivatives
- Fixed Income
- Real-Time
- Reference Data
- Brazil
---
