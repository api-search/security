---
api_specs:
- filename: uc-davis-access-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Access API
  slug: uc-davis-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-access-api-openapi.yml
- filename: uc-davis-documents-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Documents API
  slug: uc-davis-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-documents-api-openapi.yml
- filename: uc-davis-equipment-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Equipment API
  slug: uc-davis-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-equipment-api-openapi.yml
- filename: uc-davis-keys-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Keys API
  slug: uc-davis-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keys-api-openapi.yml
- filename: uc-davis-keyserials-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — KeySerials API
  slug: uc-davis-keyserials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keyserials-api-openapi.yml
- filename: uc-davis-people-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — People API
  slug: uc-davis-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-people-api-openapi.yml
- filename: uc-davis-peopleadmin-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — PeopleAdmin API
  slug: uc-davis-peopleadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-peopleadmin-api-openapi.yml
- filename: uc-davis-spaces-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Spaces API
  slug: uc-davis-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-spaces-api-openapi.yml
- filename: uc-davis-workstations-api-openapi.yml
  format: yaml
  label: PEAKS (CAES) — Workstations API
  slug: uc-davis-workstations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-workstations-api-openapi.yml
- filename: uc-davis-collection-api-openapi.yml
  format: yaml
  label: University of California, Davis Collection API
  slug: uc-davis-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-collection-api-openapi.yml
- filename: uc-davis-expert-api-openapi.yml
  format: yaml
  label: University of California, Davis Expert API
  slug: uc-davis-expert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-expert-api-openapi.yml
- filename: uc-davis-item-api-openapi.yml
  format: yaml
  label: University of California, Davis Item API
  slug: uc-davis-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-item-api-openapi.yml
- filename: uc-davis-page-search-api-openapi.yml
  format: yaml
  label: University of California, Davis page search API
  slug: uc-davis-page-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-page-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ucdavis.edu
  spf: true
hosts:
- cert_expires: Sep  5 13:27:19 2026 GMT
  host: www.ucdavis.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: iet-ws.ucdavis.edu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: health.ucdavis.edu
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uc Davis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Davis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of California, Davis
provider_slug: uc-davis
slug: uc-davis-domain-security
source_filename: uc-davis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucdavis.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:27:19 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: iet-ws.ucdavis.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: health.ucdavis.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: ucdavis.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/security/uc-davis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Research
- Research Data
- Identity Federation
- Digital Collections
- Library
- Health
- Open-Source
---
