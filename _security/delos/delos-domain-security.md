---
api_specs:
- filename: delos-actions-api-openapi.yml
  format: yaml
  label: Delos Actions API
  slug: delos-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-actions-api-openapi.yml
- filename: delos-admin-installations-api-openapi.yml
  format: yaml
  label: Delos Admin/installations API
  slug: delos-admin-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-installations-api-openapi.yml
- filename: delos-admin-products-api-openapi.yml
  format: yaml
  label: Delos Admin/products API
  slug: delos-admin-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-products-api-openapi.yml
- filename: delos-admin-products-bundles-api-openapi.yml
  format: yaml
  label: Delos Admin/products Bundles API
  slug: delos-admin-products-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-products-bundles-api-openapi.yml
- filename: delos-admin-users-api-openapi.yml
  format: yaml
  label: Delos Admin/users API
  slug: delos-admin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-admin-users-api-openapi.yml
- filename: delos-global-api-openapi.yml
  format: yaml
  label: Delos Global API
  slug: delos-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-global-api-openapi.yml
- filename: delos-installations-api-openapi.yml
  format: yaml
  label: Delos Installations API
  slug: delos-installations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-installations-api-openapi.yml
- filename: delos-local-accounts-api-openapi.yml
  format: yaml
  label: Delos Local Accounts API
  slug: delos-local-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-local-accounts-api-openapi.yml
- filename: delos-products-api-openapi.yml
  format: yaml
  label: Delos Products API
  slug: delos-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-products-api-openapi.yml
- filename: delos-sessions-api-openapi.yml
  format: yaml
  label: Delos Sessions API
  slug: delos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-sessions-api-openapi.yml
- filename: delos-users-api-openapi.yml
  format: yaml
  label: Delos Users API
  slug: delos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/openapi/delos-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: delos.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wellcube.io
  spf: false
hosts:
- cert_expires: Sep 21 08:02:09 2026 GMT
  host: delos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 06:33:48 2026 GMT
  host: wellcube.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: cloud.wellcube.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Delos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Delos, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Delos
provider_slug: delos
slug: delos-domain-security
source_filename: delos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: delos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:02:09 2026 GMT\n  hsts: false\n- host: wellcube.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 06:33:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.wellcube.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: delos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wellcube.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delos/refs/heads/main/security/delos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- wellness-real-estate
- indoor-air-quality
- indoor-environmental-quality
- iot
- smart-buildings
- building-automation
- air-purification
- environmental-sensors
- commercial-real-estate
- healthy-buildings
- hospitality
- ESG
---
