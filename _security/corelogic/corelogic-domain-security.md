---
api_specs:
- filename: corelogic-trestle-reso-web-api-openapi.yml
  format: yaml
  label: Trestle RESO Web API
  slug: trestle-reso-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-trestle-reso-web-api-openapi.yml
- filename: corelogic-direct-webapi-crm-openapi.yml
  format: yaml
  label: Direct Web API — CRM
  slug: direct-webapi-crm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/openapi/corelogic-direct-webapi-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cotality.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corelogic.com
  spf: true
hosts:
- cert_expires: Oct  7 04:27:56 2026 GMT
  host: www.cotality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: trestle-documentation.corelogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 01:22:44 2026 GMT
  host: api.cotality.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corelogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreLogic (Cotality), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoreLogic (Cotality)
provider_slug: corelogic
slug: corelogic-domain-security
source_filename: corelogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cotality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:27:56 2026 GMT\n  hsts: false\n- host: trestle-documentation.corelogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.cotality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:22:44 2026 GMT\n  hsts: null\ndomains:\n- domain: cotality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: corelogic.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic/refs/heads/main/security/corelogic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Climate Risk
- CoreLogic
- Cotality
- Direct Web API
- Hazard Data
- Insurance Data
- Listings
- Matrix MLS
- Mortgage Data
- MLS
- OData
- OneHome
- OpenID Connect
- Participant Reporting
- Property Data
- Real Estate
- RESO Data Dictionary
- RESO Web API
- RETS
- Tax Data
- Trestle
---
