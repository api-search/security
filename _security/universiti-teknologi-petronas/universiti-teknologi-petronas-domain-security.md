---
api_specs:
- filename: universiti-teknologi-petronas-discovery-api-openapi.yml
  format: yaml
  label: Universiti Teknologi PETRONAS Discovery API
  slug: universiti-teknologi-petronas-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-discovery-api-openapi.yml
- filename: universiti-teknologi-petronas-eprints-rest-api-openapi.yml
  format: yaml
  label: Universiti Teknologi PETRONAS EPrints REST API
  slug: universiti-teknologi-petronas-eprints-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-eprints-rest-api-openapi.yml
- filename: universiti-teknologi-petronas-export-api-openapi.yml
  format: yaml
  label: Universiti Teknologi PETRONAS Export API
  slug: universiti-teknologi-petronas-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-export-api-openapi.yml
- filename: universiti-teknologi-petronas-oai-pmh-api-openapi.yml
  format: yaml
  label: Universiti Teknologi PETRONAS OAI PMH API
  slug: universiti-teknologi-petronas-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-oai-pmh-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: utp.edu.my
  spf: true
hosts:
- cert_expires: Jan 19 09:48:37 2027 GMT
  host: www.utp.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 19 09:48:37 2027 GMT
  host: utpedia.utp.edu.my
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Universiti Teknologi Petronas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universiti Teknologi PETRONAS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Universiti Teknologi PETRONAS
provider_slug: universiti-teknologi-petronas
slug: universiti-teknologi-petronas-domain-security
source_filename: universiti-teknologi-petronas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.utp.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 09:48:37 2027 GMT\n  hsts: false\n- host: utpedia.utp.edu.my\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 09:48:37 2027 GMT\n  hsts: false\ndomains:\n- domain: utp.edu.my\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/security/universiti-teknologi-petronas-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- University
- Higher Education
- Education
- Malaysia
- Private Research University
- Research
- Research Repository
- Institutional Repository
- Open Access
- OAI-PMH
- EPrints
- Identity Federation
- Learning Management
- Scholarly Publishing
---
