---
api_specs:
- filename: university-of-groningen-academic-years-api-openapi.yml
  format: yaml
  label: University of Groningen Academic Years API
  slug: university-of-groningen-academic-years-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-academic-years-api-openapi.yml
- filename: university-of-groningen-courses-api-openapi.yml
  format: yaml
  label: University of Groningen Courses API
  slug: university-of-groningen-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-courses-api-openapi.yml
- filename: university-of-groningen-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Groningen OAI PMH API
  slug: university-of-groningen-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-oai-pmh-api-openapi.yml
- filename: university-of-groningen-option-lists-api-openapi.yml
  format: yaml
  label: University of Groningen Option Lists API
  slug: university-of-groningen-option-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-option-lists-api-openapi.yml
- filename: university-of-groningen-organization-api-openapi.yml
  format: yaml
  label: University of Groningen Organization API
  slug: university-of-groningen-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-organization-api-openapi.yml
- filename: university-of-groningen-programmes-api-openapi.yml
  format: yaml
  label: University of Groningen Programmes API
  slug: university-of-groningen-programmes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-programmes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rug.nl
  spf: true
- caa:
  - 0 issuewild "harica.gr"
  - 0 issue "letsencrypt.org"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:knawnet@knaw.nl"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dataverse.nl
  spf: true
hosts:
- cert_expires: Dec  1 08:48:18 2026 GMT
  host: www.rug.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 00:12:47 2026 GMT
  host: pure.rug.nl
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 12:19:21 2026 GMT
  host: dataverse.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: University Of Groningen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Groningen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Groningen
provider_slug: university-of-groningen
slug: university-of-groningen-domain-security
source_filename: university-of-groningen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rug.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:48:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pure.rug.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 00:12:47 2026 GMT\n  hsts: null\n- host: dataverse.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:19:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rug.nl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: dataverse.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:knawnet@knaw.nl\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/security/university-of-groningen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Netherlands
- Europe
- Research
- Research Data
- Course Catalog
- Identity Federation
- OAI-PMH
- Library
- Metadata
- Open Data
---
