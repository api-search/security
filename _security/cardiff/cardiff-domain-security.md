---
api_specs:
- filename: cardiff-courses-api-openapi.yml
  format: yaml
  label: Cardiff University Courses API
  slug: cardiff-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-courses-api-openapi.yml
- filename: cardiff-clearing-adjustments-api-openapi.yml
  format: yaml
  label: Cardiff University Clearing Adjustments API
  slug: cardiff-clearing-adjustments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-clearing-adjustments-api-openapi.yml
- filename: cardiff-groups-api-openapi.yml
  format: yaml
  label: Cardiff University Groups API
  slug: cardiff-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-groups-api-openapi.yml
- filename: cardiff-modules-api-openapi.yml
  format: yaml
  label: Cardiff University Modules API
  slug: cardiff-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-modules-api-openapi.yml
- filename: cardiff-assessments-api-openapi.yml
  format: yaml
  label: Cardiff University Assessments API
  slug: cardiff-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-assessments-api-openapi.yml
- filename: cardiff-occurrences-api-openapi.yml
  format: yaml
  label: Cardiff University Occurrences API
  slug: cardiff-occurrences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-occurrences-api-openapi.yml
- filename: cardiff-rollover-api-openapi.yml
  format: yaml
  label: Cardiff University Rollover API
  slug: cardiff-rollover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-rollover-api-openapi.yml
- filename: cardiff-schools-api-openapi.yml
  format: yaml
  label: Cardiff University Schools API
  slug: cardiff-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-schools-api-openapi.yml
- filename: cardiff-subjects-api-openapi.yml
  format: yaml
  label: Cardiff University Subjects API
  slug: cardiff-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-subjects-api-openapi.yml
- filename: cardiff-levels-api-openapi.yml
  format: yaml
  label: Cardiff University Levels API
  slug: cardiff-levels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-levels-api-openapi.yml
- filename: cardiff-semesters-api-openapi.yml
  format: yaml
  label: Cardiff University Semesters API
  slug: cardiff-semesters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-semesters-api-openapi.yml
- filename: cardiff-qualifications-api-openapi.yml
  format: yaml
  label: Cardiff University Qualifications API
  slug: cardiff-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-qualifications-api-openapi.yml
- filename: cardiff-years-api-openapi.yml
  format: yaml
  label: Cardiff University Years API
  slug: cardiff-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-years-api-openapi.yml
- filename: cardiff-publications-api-openapi.yml
  format: yaml
  label: Cardiff University Publications API
  slug: cardiff-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-publications-api-openapi.yml
- filename: cardiff-default-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Default API
  slug: cardiff-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-default-api-openapi.yml
- filename: cardiff-test-api-openapi.yml
  format: yaml
  label: Cardiff University Echo Test API
  slug: cardiff-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/openapi/cardiff-test-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cardiff.ac.uk
  spf: true
hosts:
- cert_expires: Sep  2 00:49:21 2026 GMT
  host: www.cardiff.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:14:17 2026 GMT
  host: data.cardiff.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: api.data.cardiff.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardiff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardiff University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cardiff University
provider_slug: cardiff
slug: cardiff-domain-security
source_filename: cardiff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 00:49:21 2026 GMT\n  hsts: null\n- host: data.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 02:14:17 2026 GMT\n  hsts: null\n- host: api.data.cardiff.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cardiff.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardiff/refs/heads/main/security/cardiff-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Public Research University
- United Kingdom
- Wales
- Russell Group
- Open Data
- Course Catalog
- Research Repository
- Identity Federation
- Research Computing
- Publications
---
