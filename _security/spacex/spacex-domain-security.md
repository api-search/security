---
api_specs:
- filename: spacex-rest-api-openapi.yml
  format: yaml
  label: SpaceX REST API (v4 + v5)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: spacexdata.com
  spf: false
hosts:
- cert_expires: Sep  4 22:27:28 2026 GMT
  host: api.spacexdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpaceX (Community API), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: SpaceX (Community API)
provider_slug: spacex
slug: spacex-domain-security
source_filename: spacex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.spacexdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:27:28 2026 GMT\n  hsts: null\ndomains:\n- domain: spacexdata.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/security/spacex-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Space
- Launch
- Satellites
- Starlink
- Falcon 9
- Falcon Heavy
- Dragon
- Rockets
- Open Source
- Community
- REST
- GraphQL
- Open Data
---
