---
api_specs:
- filename: university-of-lisbon-campus-life-api-openapi.yml
  format: yaml
  label: University of Lisbon Campus Life API
  slug: university-of-lisbon-campus-life-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-campus-life-api-openapi.yml
- filename: university-of-lisbon-courses-api-openapi.yml
  format: yaml
  label: University of Lisbon Courses API
  slug: university-of-lisbon-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-courses-api-openapi.yml
- filename: university-of-lisbon-degrees-api-openapi.yml
  format: yaml
  label: University of Lisbon Degrees API
  slug: university-of-lisbon-degrees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-degrees-api-openapi.yml
- filename: university-of-lisbon-domain-model-api-openapi.yml
  format: yaml
  label: University of Lisbon Domain Model API
  slug: university-of-lisbon-domain-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-domain-model-api-openapi.yml
- filename: university-of-lisbon-institution-api-openapi.yml
  format: yaml
  label: University of Lisbon Institution API
  slug: university-of-lisbon-institution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-institution-api-openapi.yml
- filename: university-of-lisbon-person-api-openapi.yml
  format: yaml
  label: University of Lisbon Person API
  slug: university-of-lisbon-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-person-api-openapi.yml
- filename: university-of-lisbon-spaces-api-openapi.yml
  format: yaml
  label: University of Lisbon Spaces API
  slug: university-of-lisbon-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/openapi/university-of-lisbon-spaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ulisboa.pt
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fenixedu.org
  spf: true
hosts:
- cert_expires: Jan 10 03:14:55 2027 GMT
  host: www.ulisboa.pt
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 04:24:37 2026 GMT
  host: fenixedu.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 15:59:46 2026 GMT
  host: fenix.tecnico.ulisboa.pt
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: University Of Lisbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Lisbon, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: University of Lisbon
provider_slug: university-of-lisbon
slug: university-of-lisbon-domain-security
source_filename: university-of-lisbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ulisboa.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 03:14:55 2027 GMT\n  hsts: false\n- host: fenixedu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 04:24:37 2026 GMT\n  hsts: false\n- host: fenix.tecnico.ulisboa.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:59:46 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: ulisboa.pt\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fenixedu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-lisbon/refs/heads/main/security/university-of-lisbon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Portugal
- Europe
- Public Research University
- Course Catalog
- Research Repository
- Library
- Identity Federation
- OAI-PMH
- Open Access
- Erasmus Without Paper
- Metadata
---
