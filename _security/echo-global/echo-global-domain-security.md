---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: EchoSync Partner-Connect API
  slug: echosync-partner-connect-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/echogl/rest-api/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Customer API
  slug: echosync-customer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Customer_API_OAuth_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Carrier API
  slug: echosync-carrier-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Carrier_API_Public/
- filename: openapi.yaml
  format: yaml
  label: EchoSync Authorizer API
  slug: echosync-authorizer-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis-docs/echogl/Echo_Authorizer_Public/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: echo.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Oct  5 09:28:03 2026 GMT
  host: www.echo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.echo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: virtserver.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echo Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo Global Logistics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Echo Global Logistics
provider_slug: echo-global
slug: echo-global-domain-security
source_filename: echo-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 09:28:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.echo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\n- host: virtserver.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: echo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo-global/refs/heads/main/security/echo-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Logistics
- Shipping
- LTL
- Truckload
- Freight Brokerage
- Transportation
- Supply Chain
---
