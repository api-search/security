---
api_specs:
- filename: national-university-of-colombia-oai-pmh-api-openapi.yml
  format: yaml
  label: National University of Colombia OAI-PMH API
  slug: national-university-of-colombia-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-university-of-colombia/refs/heads/main/openapi/national-university-of-colombia-oai-pmh-api-openapi.yml
- filename: national-university-of-colombia-rest-core-api-openapi.yml
  format: yaml
  label: National University of Colombia REST - Core API
  slug: national-university-of-colombia-rest-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-university-of-colombia/refs/heads/main/openapi/national-university-of-colombia-rest-core-api-openapi.yml
- filename: national-university-of-colombia-rest-discover-api-openapi.yml
  format: yaml
  label: National University of Colombia REST - Discover API
  slug: national-university-of-colombia-rest-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-university-of-colombia/refs/heads/main/openapi/national-university-of-colombia-rest-discover-api-openapi.yml
- filename: national-university-of-colombia-journals-oai-pmh-api-openapi.yml
  format: yaml
  label: National University of Colombia Portal de Revistas UN OAI-PMH API
  slug: national-university-of-colombia-journals-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-university-of-colombia/refs/heads/main/openapi/national-university-of-colombia-journals-oai-pmh-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unal.edu.co
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: unal.edu.co
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: repositorio.unal.edu.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: bffrepositorio.unal.edu.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National University Of Colombia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National University of Colombia, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: National University of Colombia
provider_slug: national-university-of-colombia
slug: national-university-of-colombia-domain-security
source_filename: national-university-of-colombia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unal.edu.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: repositorio.unal.edu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: bffrepositorio.unal.edu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: unal.edu.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-university-of-colombia/refs/heads/main/security/national-university-of-colombia-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Public Research University
- Colombia
- Latin America
- Open Data
- Institutional Repository
- Research Data
- Scholarly Publishing
- Library
- OAI-PMH
---
