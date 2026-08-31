---
api_specs:
- filename: elisa-categories-api-openapi.yml
  format: yaml
  label: ELISA Categories API
  slug: elisa-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-categories-api-openapi.yml
- filename: elisa-doc-api-openapi.yml
  format: yaml
  label: ELISA Doc API
  slug: elisa-doc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-doc-api-openapi.yml
- filename: elisa-events-api-openapi.yml
  format: yaml
  label: ELISA Events API
  slug: elisa-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-events-api-openapi.yml
- filename: elisa-organizers-api-openapi.yml
  format: yaml
  label: ELISA Organizers API
  slug: elisa-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-organizers-api-openapi.yml
- filename: elisa-tags-api-openapi.yml
  format: yaml
  label: ELISA Tags API
  slug: elisa-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-tags-api-openapi.yml
- filename: elisa-venues-api-openapi.yml
  format: yaml
  label: ELISA Venues API
  slug: elisa-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/openapi/elisa-venues-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elisa.tech
  spf: true
hosts:
- cert_expires: Nov  5 17:59:39 2026 GMT
  host: elisa.tech
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elisa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ELISA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ELISA
provider_slug: elisa
slug: elisa-domain-security
source_filename: elisa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elisa.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: elisa.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elisa/refs/heads/main/security/elisa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Embedded
- Linux
- Linux Foundation
- Safety
- Functional Safety
- Open Source
- Automotive
- Aerospace
- Medical Devices
- Traceability
- Standards
- Events
---
