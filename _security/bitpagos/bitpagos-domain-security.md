---
api_specs:
- filename: bitpagos-bitpagos-api-api-openapi.yml
  format: yaml
  label: Bitpagos Bitpagos API
  slug: bitpagos-bitpagos-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-bitpagos-api-api-openapi.yml
- filename: bitpagos-customers-api-openapi.yml
  format: yaml
  label: Bitpagos Customers API
  slug: bitpagos-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-customers-api-openapi.yml
- filename: bitpagos-offramp-api-openapi.yml
  format: yaml
  label: Bitpagos Offramp API
  slug: bitpagos-offramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-offramp-api-openapi.yml
- filename: bitpagos-quotes-api-openapi.yml
  format: yaml
  label: Bitpagos Quotes API
  slug: bitpagos-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-quotes-api-openapi.yml
- filename: bitpagos-rates-api-openapi.yml
  format: yaml
  label: Bitpagos Rates API
  slug: bitpagos-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-rates-api-openapi.yml
- filename: bitpagos-resources-api-openapi.yml
  format: yaml
  label: Bitpagos Resources API
  slug: bitpagos-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-resources-api-openapi.yml
- filename: bitpagos-trade-api-openapi.yml
  format: yaml
  label: Bitpagos Trade API
  slug: bitpagos-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/openapi/bitpagos-trade-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ripio.com
  spf: true
hosts:
- cert_expires: Dec 10 04:00:45 2026 GMT
  host: www.ripio.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 04:00:45 2026 GMT
  host: docs.ripio.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 04:00:45 2026 GMT
  host: b2b-api.ripio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bitpagos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitpagos, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bitpagos
provider_slug: bitpagos
slug: bitpagos-domain-security
source_filename: bitpagos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ripio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.ripio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:00:45 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: b2b-api.ripio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 04:00:45 2026 GMT\n  hsts: null\ndomains:\n- domain: ripio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpagos/refs/heads/main/security/bitpagos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Fintech
- Latin America
- Bitcoin
- Credit Cards
---
