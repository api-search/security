---
api_specs:
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Link / Connect API
  slug: flexpa-link-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa FHIR Resources API
  slug: flexpa-fhir-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flexpa.com
  spf: true
hosts:
- cert_expires: Sep 22 20:10:11 2026 GMT
  host: www.flexpa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: api.flexpa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flexpa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexpa, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flexpa
provider_slug: flexpa
slug: flexpa-domain-security
source_filename: flexpa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flexpa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:10:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.flexpa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flexpa.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/security/flexpa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
---
