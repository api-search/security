---
api_specs:
- filename: university-of-wisconsin-madison-person-api-openapi.yml
  format: yaml
  label: Person API
  slug: person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-openapi.yml
  format: yaml
  label: Mock Person API
  slug: mock-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
  format: yaml
  label: Mock Person API (Certificates)
  slug: mock-person-api-certificates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
- filename: university-of-wisconsin-madison-hr-api-openapi.yml
  format: yaml
  label: HR API
  slug: hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-hr-api-openapi.yml
  format: yaml
  label: Mock HR API
  slug: mock-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-manifest-api-openapi.yml
  format: yaml
  label: Manifest API
  slug: manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-manifest-api-openapi.yml
  format: yaml
  label: Mock Manifest API
  slug: mock-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-finance-api-openapi.yml
  format: yaml
  label: Finance API
  slug: finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-finance-api-openapi.yml
- filename: university-of-wisconsin-madison-locations-api-openapi.yml
  format: yaml
  label: Locations API
  slug: locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-locations-api-openapi.yml
- filename: university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
  format: yaml
  label: Enterprise Billing API
  slug: enterprise-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
- filename: university-of-wisconsin-madison-oauth-api-openapi.yml
  format: yaml
  label: OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-oauth-api-openapi.yml
- filename: university-of-wisconsin-madison-course-search-api-openapi.yml
  format: yaml
  label: Public Course Search API
  slug: course-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-course-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wisc.edu
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.wisc.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 02:52:46 2026 GMT
  host: developer.wisc.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 15:17:39 2026 GMT
  host: wams.doit.wisc.edu
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Wisconsin Madison Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Wisconsin-Madison, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Wisconsin-Madison
provider_slug: university-of-wisconsin-madison
slug: university-of-wisconsin-madison-domain-security
source_filename: university-of-wisconsin-madison-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wisc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\n- host: developer.wisc.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:52:46 2026 GMT\n  hsts: null\n- host: wams.doit.wisc.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 15:17:39 2026 GMT\n  hsts: false\ndomains:\n- domain: wisc.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/security/university-of-wisconsin-madison-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Wisconsin
- Big Ten
- Association of American Universities
- Identity
- Identity Federation
- Course Catalog
- Research Repository
- Student Information System
- Human Resources
- Finance
- Curriculum
---
