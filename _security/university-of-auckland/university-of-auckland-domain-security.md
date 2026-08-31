---
api_specs:
- filename: university-of-auckland-course-catalog-v3-openapi.yml
  format: yaml
  label: University of Auckland Course Catalog Api V3
  slug: course-catalog-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-course-catalog-v3-openapi.yml
- filename: university-of-auckland-classes-v2-openapi.yml
  format: yaml
  label: University of Auckland Classes Api V2
  slug: classes-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/openapi/university-of-auckland-classes-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auckland.ac.nz
  spf: true
hosts:
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: www.auckland.ac.nz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: developer.auckland.ac.nz
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: apis.auckland.ac.nz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Auckland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Auckland, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Auckland
provider_slug: university-of-auckland
slug: university-of-auckland-domain-security
source_filename: university-of-auckland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auckland.ac.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.auckland.ac.nz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\n- host: apis.auckland.ac.nz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: auckland.ac.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-auckland/refs/heads/main/security/university-of-auckland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- New Zealand
- Public Research University
- Universitas 21
- Course Catalog
- Student Records
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
---
