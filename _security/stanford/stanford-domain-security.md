---
api_specs:
- filename: stanford-sdr-api-openapi.yml
  format: yaml
  label: SDR API
  slug: sdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-sdr-api-openapi.yml
- filename: stanford-dor-services-api-openapi.yml
  format: yaml
  label: DOR Services API
  slug: dor-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-dor-services-api-openapi.yml
- filename: stanford-preservation-catalog-api-openapi.yml
  format: yaml
  label: Preservation Catalog HTTP API
  slug: preservation-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-preservation-catalog-api-openapi.yml
- filename: stanford-technical-metadata-api-openapi.yml
  format: yaml
  label: Technical Metadata API
  slug: technical-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-technical-metadata-api-openapi.yml
- filename: stanford-suri-api-openapi.yml
  format: yaml
  label: SURI API
  slug: suri-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-suri-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stanford.edu
  spf: true
hosts:
- cert_expires: Sep 23 14:19:11 2026 GMT
  host: www.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 10:53:43 2026 GMT
  host: api.library.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: purl.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stanford Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stanford University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stanford University
provider_slug: stanford
slug: stanford-domain-security
source_filename: stanford-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stanford.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:19:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.library.stanford.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: purl.stanford.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stanford.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/security/stanford-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Research
- United States
- California
- Private Research University
- Association of American Universities
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Digital Repository
- Artificial Intelligence
- IIIF
---
