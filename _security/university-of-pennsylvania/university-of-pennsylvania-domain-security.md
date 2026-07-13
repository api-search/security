---
api_specs:
- filename: university-of-pennsylvania-penn-courses.yaml
  format: yaml
  label: Penn Courses (PCX) API
  slug: penn-courses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/openapi/university-of-pennsylvania-penn-courses.yaml
- filename: university-of-pennsylvania-penn-courses.yaml
  format: yaml
  label: Penn Course Review API
  slug: penn-course-review
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/openapi/university-of-pennsylvania-penn-courses.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: upenn.edu
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pennlabs.org
  spf: false
hosts:
- cert_expires: Sep  7 19:15:27 2026 GMT
  host: www.upenn.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:57:44 2026 GMT
  host: pennlabs.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: penn-sdk.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Pennsylvania Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Pennsylvania, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Pennsylvania
provider_slug: university-of-pennsylvania
slug: university-of-pennsylvania-domain-security
source_filename: university-of-pennsylvania-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upenn.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:15:27 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: pennlabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:57:44 2026 GMT\n  hsts: false\n- host: penn-sdk.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upenn.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pennlabs.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/security/university-of-pennsylvania-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Courses
- Library
- United States
- Ivy League
---
