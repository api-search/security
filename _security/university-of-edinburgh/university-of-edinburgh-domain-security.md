---
api_specs:
- filename: university-of-edinburgh-elm-api-openapi.yml
  format: yaml
  label: ELM — Edinburgh Language Models API
  slug: elm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-elm-api-openapi.yml
- filename: university-of-edinburgh-catalogue-api-openapi.yml
  format: yaml
  label: University of Edinburgh Catalogue API
  slug: university-of-edinburgh-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-catalogue-api-openapi.yml
- filename: university-of-edinburgh-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Edinburgh OAI PMH API
  slug: university-of-edinburgh-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-oai-pmh-api-openapi.yml
- filename: university-of-edinburgh-repository-api-openapi.yml
  format: yaml
  label: University of Edinburgh Repository API
  slug: university-of-edinburgh-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/openapi/university-of-edinburgh-repository-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ed.ac.uk
  spf: true
hosts:
- cert_expires: Aug 26 00:22:30 2026 GMT
  host: www.ed.ac.uk
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 11:03:32 2026 GMT
  host: libraryblogs.is.ed.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 02:44:00 2026 GMT
  host: datashare.ed.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Edinburgh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Edinburgh, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Edinburgh
provider_slug: university-of-edinburgh
slug: university-of-edinburgh-domain-security
source_filename: university-of-edinburgh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ed.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:22:30 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: libraryblogs.is.ed.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  2 11:03:32 2026 GMT\n  hsts: false\n- host: datashare.ed.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 02:44:00 2026 GMT\n  hsts: false\ndomains:\n- domain: ed.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-edinburgh/refs/heads/main/security/university-of-edinburgh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United Kingdom
- Scotland
- Russell Group
- Research Repository
- Open Data
- Identity Federation
- Research Computing
- OAI-PMH
- Artificial Intelligence
---
