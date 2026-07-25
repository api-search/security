---
api_specs:
- filename: salt-edge-accounts-api-openapi.yml
  format: yaml
  label: Salt Edge Accounts API
  slug: salt-edge-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-accounts-api-openapi.yml
- filename: salt-edge-connect-sessions-api-openapi.yml
  format: yaml
  label: Salt Edge Connect Sessions API
  slug: salt-edge-connect-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-connect-sessions-api-openapi.yml
- filename: salt-edge-connections-api-openapi.yml
  format: yaml
  label: Salt Edge Connections API
  slug: salt-edge-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-connections-api-openapi.yml
- filename: salt-edge-consents-api-openapi.yml
  format: yaml
  label: Salt Edge Consents API
  slug: salt-edge-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-consents-api-openapi.yml
- filename: salt-edge-countries-api-openapi.yml
  format: yaml
  label: Salt Edge Countries API
  slug: salt-edge-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-countries-api-openapi.yml
- filename: salt-edge-customers-api-openapi.yml
  format: yaml
  label: Salt Edge Customers API
  slug: salt-edge-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-customers-api-openapi.yml
- filename: salt-edge-holder-info-api-openapi.yml
  format: yaml
  label: Salt Edge Holder Info API
  slug: salt-edge-holder-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-holder-info-api-openapi.yml
- filename: salt-edge-providers-api-openapi.yml
  format: yaml
  label: Salt Edge Providers API
  slug: salt-edge-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-providers-api-openapi.yml
- filename: salt-edge-transactions-api-openapi.yml
  format: yaml
  label: Salt Edge Transactions API
  slug: salt-edge-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/openapi/salt-edge-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "rapidssl.com"
  - 0 issue "d-trust.net"
  - 0 issuewild "comodoca.com"
  - 0 issue "rapidssl.com"
  - 0 issue "actalis.it"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saltedge.com
  spf: true
hosts:
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: www.saltedge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 21 23:59:59 2027 GMT
  host: docs.saltedge.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Salt Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salt Edge, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Salt Edge
provider_slug: salt-edge
slug: salt-edge-domain-security
source_filename: salt-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saltedge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.saltedge.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: saltedge.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"rapidssl.com\"\n  - 0 issue \"d-trust.net\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"actalis.it\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salt-edge/refs/heads/main/security/salt-edge-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fintech
- Open Banking
- PSD2
- Aggregator
- Global
- AISP
- PISP
- Compliance
- AML
---
