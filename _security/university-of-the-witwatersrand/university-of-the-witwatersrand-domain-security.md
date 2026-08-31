---
api_specs:
- filename: university-of-the-witwatersrand-root-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Root API
  slug: university-of-the-witwatersrand-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-root-api-openapi.yml
- filename: university-of-the-witwatersrand-communities-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Communities API
  slug: university-of-the-witwatersrand-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-communities-api-openapi.yml
- filename: university-of-the-witwatersrand-collections-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Collections API
  slug: university-of-the-witwatersrand-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-collections-api-openapi.yml
- filename: university-of-the-witwatersrand-items-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Items API
  slug: university-of-the-witwatersrand-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-items-api-openapi.yml
- filename: university-of-the-witwatersrand-discovery-api-openapi.yml
  format: yaml
  label: WIReDSpace DSpace REST Discovery API
  slug: university-of-the-witwatersrand-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-discovery-api-openapi.yml
- filename: university-of-the-witwatersrand-request-api-openapi.yml
  format: yaml
  label: WIReDSpace OAI-PMH Interface
  slug: university-of-the-witwatersrand-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-request-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wits.ac.za
  spf: true
hosts:
- cert_expires: Feb 13 12:46:08 2027 GMT
  host: www.wits.ac.za
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  6 23:46:19 2027 GMT
  host: wiredspace.wits.ac.za
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: opendata.wits.ac.za
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of The Witwatersrand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of the Witwatersrand, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of the Witwatersrand
provider_slug: university-of-the-witwatersrand
slug: university-of-the-witwatersrand-domain-security
source_filename: university-of-the-witwatersrand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wits.ac.za\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 12:46:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wiredspace.wits.ac.za\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  6 23:46:19 2027 GMT\n  hsts: false\n- host: opendata.wits.ac.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: wits.ac.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/security/university-of-the-witwatersrand-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Research
- South Africa
- Africa
- Institutional Repository
- Research Data
- Open Access
- Identity Federation
- OAI-PMH
- DSpace
---
