---
api_specs:
- filename: solera-assignment-api-openapi.yml
  format: yaml
  label: Solera Assignment API
  slug: solera-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-assignment-api-openapi.yml
- filename: solera-estimatereturn-api-openapi.yml
  format: yaml
  label: Solera Estimate Return API
  slug: solera-estimatereturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-estimatereturn-api-openapi.yml
- filename: solera-getclaimimageresponse-api-openapi.yml
  format: yaml
  label: Solera Get Claim Image Response API
  slug: solera-getclaimimageresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getclaimimageresponse-api-openapi.yml
- filename: solera-getdocument-api-openapi.yml
  format: yaml
  label: Solera Get Document API
  slug: solera-getdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocument-api-openapi.yml
- filename: solera-getdocuments-api-openapi.yml
  format: yaml
  label: Solera Get Documents API
  slug: solera-getdocuments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getdocuments-api-openapi.yml
- filename: solera-getimage-api-openapi.yml
  format: yaml
  label: Solera Get Image API
  slug: solera-getimage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getimage-api-openapi.yml
- filename: solera-getvaluation-api-openapi.yml
  format: yaml
  label: Solera Get Valuation API
  slug: solera-getvaluation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluation-api-openapi.yml
- filename: solera-getvaluationresponse-api-openapi.yml
  format: yaml
  label: Solera Get Valuation Response API
  slug: solera-getvaluationresponse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-getvaluationresponse-api-openapi.yml
- filename: solera-gicintegration-api-openapi.yml
  format: yaml
  label: Solera GIC Integration API
  slug: solera-gicintegration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-gicintegration-api-openapi.yml
- filename: solera-valuationreturn-api-openapi.yml
  format: yaml
  label: Solera Valuation Return API
  slug: solera-valuationreturn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-valuationreturn-api-openapi.yml
- filename: solera-version-api-openapi.yml
  format: yaml
  label: Solera Version API
  slug: solera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/openapi/solera-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "ssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: solera.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audatex.com
  spf: true
hosts:
- cert_expires: Oct 19 09:48:03 2026 GMT
  host: www.solera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api-demo.audatex.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Solera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solera, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Solera
provider_slug: solera
slug: solera-domain-security
source_filename: solera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 09:48:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-demo.audatex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: solera.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: audatex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solera/refs/heads/main/security/solera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United States
- Property and Casualty
- Claims
- Claims Technology
- Automotive Claims
- FNOL
- Vehicle Damage Assessment
- Risk Data
- CIECA
- Insurtech
---
