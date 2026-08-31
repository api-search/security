---
api_specs:
- filename: university-of-warwick-administration-api-openapi.yml
  format: yaml
  label: University of Warwick Administration API
  slug: university-of-warwick-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-administration-api-openapi.yml
- filename: university-of-warwick-jobs-api-openapi.yml
  format: yaml
  label: University of Warwick Jobs API
  slug: university-of-warwick-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-jobs-api-openapi.yml
- filename: university-of-warwick-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Warwick OAI PMH API
  slug: university-of-warwick-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-oai-pmh-api-openapi.yml
- filename: university-of-warwick-timetabling-api-openapi.yml
  format: yaml
  label: University of Warwick Timetabling API
  slug: university-of-warwick-timetabling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-timetabling-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "quovadisglobal.com"
  - 0 issue "geotrust.com"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: warwick.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: warwicksu.com
  spf: true
hosts:
- cert_expires: Oct  2 22:08:48 2026 GMT
  host: warwick.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 03:18:44 2026 GMT
  host: tabula.warwick.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.warwicksu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Warwick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Warwick, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Warwick
provider_slug: university-of-warwick
slug: university-of-warwick-domain-security
source_filename: university-of-warwick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: warwick.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:08:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tabula.warwick.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:18:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.warwicksu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: warwick.ac.uk\n  dnssec: false\n  caa:\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: warwicksu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/security/university-of-warwick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Identity Federation
- Research Repository
- Course Catalog
- Timetabling
- Student Information System
- Open Data
---
