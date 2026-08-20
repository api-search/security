---
api_specs:
- filename: digital-asset-common-api-openapi.yml
  format: yaml
  label: Digital Asset Common API
  slug: digital-asset-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-common-api-openapi.yml
- filename: digital-asset-operator-api-openapi.yml
  format: yaml
  label: Digital Asset Operator API
  slug: digital-asset-operator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-operator-api-openapi.yml
- filename: digital-asset-public-api-openapi.yml
  format: yaml
  label: Digital Asset Public API
  slug: digital-asset-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-public-api-openapi.yml
- filename: digital-asset-registry-api-openapi.yml
  format: yaml
  label: Digital Asset Registry API
  slug: digital-asset-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/openapi/digital-asset-registry-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "thawte.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitalasset.com
  spf: true
hosts:
- cert_expires: Oct 11 12:30:40 2026 GMT
  host: www.digitalasset.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 15:33:48 2026 GMT
  host: docs.digitalasset.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:52:13 2026 GMT
  host: api.utilities.digitalasset.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Asset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Asset, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digital Asset
provider_slug: digital-asset
slug: digital-asset-domain-security
source_filename: digital-asset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalasset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 12:30:40 2026 GMT\n  hsts: null\n- host: docs.digitalasset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 15:33:48 2026 GMT\n  hsts: null\n- host: api.utilities.digitalasset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:52:13 2026 GMT\n  hsts: null\ndomains:\n- domain: digitalasset.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"thawte.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-asset/refs/heads/main/security/digital-asset-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Tokenization
- Digital Assets
- Financial-Services
- Distributed Ledger
- Smart Contracts
- Capital Markets
- Canton Network
- Daml
- Stablecoins
---
