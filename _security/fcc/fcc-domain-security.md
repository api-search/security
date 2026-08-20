---
api_specs:
- filename: fcc-am-pattern-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Am Pattern API
  slug: fcc-am-pattern-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-am-pattern-api-openapi.yml
- filename: fcc-antenna-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Antenna API
  slug: fcc-antenna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-antenna-api-openapi.yml
- filename: fcc-area-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Area API
  slug: fcc-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-area-api-openapi.yml
- filename: fcc-block-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Block API
  slug: fcc-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-block-api-openapi.yml
- filename: fcc-coordinate-conversion-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Coordinate Conversion API
  slug: fcc-coordinate-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-coordinate-conversion-api-openapi.yml
- filename: fcc-coverage-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Coverage API
  slug: fcc-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-coverage-api-openapi.yml
- filename: fcc-distance-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Distance API
  slug: fcc-distance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-distance-api-openapi.yml
- filename: fcc-elevation-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Elevation API
  slug: fcc-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-elevation-api-openapi.yml
- filename: fcc-entity-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Entity API
  slug: fcc-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-entity-api-openapi.yml
- filename: fcc-haat-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Haat API
  slug: fcc-haat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-haat-api-openapi.yml
- filename: fcc-profile-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Profile API
  slug: fcc-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-profile-api-openapi.yml
- filename: fcc-projection-api-openapi.yml
  format: yaml
  label: FCC (Federal Communications Commission) Projection API
  slug: fcc-projection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/openapi/fcc-projection-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fcc.gov
  spf: true
hosts:
- cert_expires: Aug 11 23:59:59 2026 GMT
  host: www.fcc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  4 01:13:20 2026 GMT
  host: data.fcc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: geo.fcc.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fcc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FCC (Federal Communications Commission), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FCC (Federal Communications Commission)
provider_slug: fcc
slug: fcc-domain-security
source_filename: fcc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fcc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 23:59:59 2026 GMT\n  hsts: null\n- host: data.fcc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 01:13:20 2026 GMT\n  hsts: null\n- host: geo.fcc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fcc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fcc/refs/heads/main/security/fcc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal-Government
- Telecommunications
- Radio
- Broadband
- Spectrum
- Licensing
- Regulatory
---
