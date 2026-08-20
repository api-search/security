---
api_specs:
- filename: yale-search-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Search API
  slug: yale-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-search-api-openapi.yml
- filename: yale-documents-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Documents API
  slug: yale-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-documents-api-openapi.yml
- filename: yale-facets-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Facets API
  slug: yale-facets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-facets-api-openapi.yml
- filename: yale-related-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Related API
  slug: yale-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-related-api-openapi.yml
- filename: yale-configuration-api-openapi.yml
  format: yaml
  label: LUX Collections Discovery — Configuration API
  slug: yale-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-configuration-api-openapi.yml
- filename: yale-dataverse-openapi.yml
  format: yaml
  label: Yale Dataverse Repository API
  slug: dataverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-dataverse-openapi.yml
- filename: yale-digital-collections-iiif-openapi.yml
  format: yaml
  label: Yale University Library Digital Collections IIIF
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-digital-collections-iiif-openapi.yml
- filename: yale-identity-federation-openapi.yml
  format: yaml
  label: Yale University Identity Federation Metadata
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/openapi/yale-identity-federation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yale.edu
  spf: true
hosts:
- cert_expires: Jul 25 04:21:54 2026 GMT
  host: www.yale.edu
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 26 14:15:33 2026 GMT
  host: developers.yale.edu
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 10:15:53 2026 GMT
  host: gw.its.yale.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yale University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yale University
provider_slug: yale
slug: yale-domain-security
source_filename: yale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yale.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 25 04:21:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: developers.yale.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:15:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: gw.its.yale.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 10:15:53 2026 GMT\n  hsts: null\ndomains:\n- domain: yale.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yale/refs/heads/main/security/yale-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United States
- Ivy League
- Research
- Research Data
- Research Repository
- Identity Federation
- Library
- Cultural Heritage
- Linked Data
- IIIF
- Course Catalog
---
