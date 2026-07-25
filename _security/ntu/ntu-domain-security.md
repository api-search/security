---
api_specs:
- filename: ntu-discover-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Discover API
  slug: ntu-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-discover-api-openapi.yml
- filename: ntu-info-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Info API
  slug: ntu-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-info-api-openapi.yml
- filename: ntu-items-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Items API
  slug: ntu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-items-api-openapi.yml
- filename: ntu-oai-pmh-api-openapi.yml
  format: yaml
  label: Nanyang Technological University OAI-PMH API
  slug: ntu-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-oai-pmh-api-openapi.yml
- filename: ntu-root-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Root API
  slug: ntu-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-root-api-openapi.yml
- filename: ntu-search-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Search API
  slug: ntu-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ntu.edu.sg
  spf: true
hosts:
- cert_expires: Aug 31 15:04:27 2026 GMT
  host: www.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 03:46:22 2026 GMT
  host: libguides.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: researchdata.ntu.edu.sg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ntu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanyang Technological University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nanyang Technological University
provider_slug: ntu
slug: ntu-domain-security
source_filename: ntu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 15:04:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: libguides.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: researchdata.ntu.edu.sg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ntu.edu.sg\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/security/ntu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Singapore
- Research Data
- Open Data
- Repository
- Library
---
