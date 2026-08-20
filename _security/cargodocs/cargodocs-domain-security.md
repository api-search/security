---
api_specs:
- filename: cargodocs-common-api-openapi.yml
  format: yaml
  label: CargoDocs Common API
  slug: cargodocs-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-common-api-openapi.yml
- filename: cargodocs-documents-api-openapi.yml
  format: yaml
  label: CargoDocs Documents API
  slug: cargodocs-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-documents-api-openapi.yml
- filename: cargodocs-exchange-api-openapi.yml
  format: yaml
  label: CargoDocs Exchange API
  slug: cargodocs-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-exchange-api-openapi.yml
- filename: cargodocs-import-api-openapi.yml
  format: yaml
  label: CargoDocs Import API
  slug: cargodocs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-import-api-openapi.yml
- filename: cargodocs-issuance-api-openapi.yml
  format: yaml
  label: CargoDocs Issuance API
  slug: cargodocs-issuance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-issuance-api-openapi.yml
- filename: cargodocs-surrender-api-openapi.yml
  format: yaml
  label: CargoDocs Surrender API
  slug: cargodocs-surrender-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-surrender-api-openapi.yml
- filename: cargodocs-transactions-api-openapi.yml
  format: yaml
  label: CargoDocs Transactions API
  slug: cargodocs-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: essdocs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.essdocs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: cargodocs-partner.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.essdocs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cargodocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CargoDocs, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CargoDocs
provider_slug: cargodocs
slug: cargodocs-domain-security
source_filename: cargodocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.essdocs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\n- host: cargodocs-partner.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.essdocs.com\n  https: false\ndomains:\n- domain: essdocs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/security/cargodocs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bills of Lading
- Documentation
- eBOL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
---
