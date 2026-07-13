---
api_specs:
- filename: cargodocs-partner-openapi.yml
  format: yaml
  label: CargoDocs Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-partner-openapi.yml
- filename: cargodocs-issuer-openapi.yml
  format: yaml
  label: CargoDocs Issuer API
  slug: issuer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-issuer-openapi.yml
- filename: cargodocs-customer-openapi.yml
  format: yaml
  label: CargoDocs Customer Data/Docs API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargodocs/refs/heads/main/openapi/cargodocs-customer-openapi.yml
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
- eBoL
- EssDocs
- MLETR
- Shipping
- Supply Chain
- Trade
- Trade Finance
- Warehouse Warrants
---
