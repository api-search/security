---
api_specs:
- filename: purdue-buildings-api-openapi.yml
  format: yaml
  label: Purdue University Buildings API
  slug: purdue-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-buildings-api-openapi.yml
- filename: purdue-campuses-api-openapi.yml
  format: yaml
  label: Purdue University Campuses API
  slug: purdue-campuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-campuses-api-openapi.yml
- filename: purdue-classes-api-openapi.yml
  format: yaml
  label: Purdue University Classes API
  slug: purdue-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-classes-api-openapi.yml
- filename: purdue-courses-api-openapi.yml
  format: yaml
  label: Purdue University Courses API
  slug: purdue-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-courses-api-openapi.yml
- filename: purdue-instructors-api-openapi.yml
  format: yaml
  label: Purdue University Instructors API
  slug: purdue-instructors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-instructors-api-openapi.yml
- filename: purdue-meetings-api-openapi.yml
  format: yaml
  label: Purdue University Meetings API
  slug: purdue-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-meetings-api-openapi.yml
- filename: purdue-rooms-api-openapi.yml
  format: yaml
  label: Purdue University Rooms API
  slug: purdue-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-rooms-api-openapi.yml
- filename: purdue-sections-api-openapi.yml
  format: yaml
  label: Purdue University Sections API
  slug: purdue-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-sections-api-openapi.yml
- filename: purdue-subjects-api-openapi.yml
  format: yaml
  label: Purdue University Subjects API
  slug: purdue-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-subjects-api-openapi.yml
- filename: purdue-terms-api-openapi.yml
  format: yaml
  label: Purdue University Terms API
  slug: purdue-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/openapi/purdue-terms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: purdue.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: purdue.io
  spf: false
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.purdue.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:39:01 2026 GMT
  host: api.purdue.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 13:59:15 2026 GMT
  host: purr.purdue.edu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Purdue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Purdue University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Purdue University
provider_slug: purdue
slug: purdue-domain-security
source_filename: purdue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.purdue.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.purdue.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:39:01 2026 GMT\n  hsts: false\n- host: purr.purdue.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:59:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: purdue.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: purdue.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purdue/refs/heads/main/security/purdue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- United States
---
