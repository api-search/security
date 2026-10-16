---
api_specs:
- filename: chloris-geospatial-aoi-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Aoi API
  slug: chloris-geospatial-aoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-aoi-api-openapi.yml
- filename: chloris-geospatial-boundary-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Boundary API
  slug: chloris-geospatial-boundary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-boundary-api-openapi.yml
- filename: chloris-geospatial-collection-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Collection API
  slug: chloris-geospatial-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-collection-api-openapi.yml
- filename: chloris-geospatial-info-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Info API
  slug: chloris-geospatial-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-info-api-openapi.yml
- filename: chloris-geospatial-invite-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Invite API
  slug: chloris-geospatial-invite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-invite-api-openapi.yml
- filename: chloris-geospatial-mgrstiles-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Mgrs Tiles API
  slug: chloris-geospatial-mgrstiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-mgrstiles-api-openapi.yml
- filename: chloris-geospatial-organization-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Organization API
  slug: chloris-geospatial-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-organization-api-openapi.yml
- filename: chloris-geospatial-reportingunit-api-openapi.yml
  format: yaml
  label: Chloris Geospatial Reporting Unit API
  slug: chloris-geospatial-reportingunit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-reportingunit-api-openapi.yml
- filename: chloris-geospatial-user-api-openapi.yml
  format: yaml
  label: Chloris Geospatial User API
  slug: chloris-geospatial-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/openapi/chloris-geospatial-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chloris.earth
  spf: true
hosts:
- cert_expires: Dec 14 18:32:05 2026 GMT
  host: www.chloris.earth
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chloris Geospatial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chloris Geospatial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chloris Geospatial
provider_slug: chloris-geospatial
slug: chloris-geospatial-domain-security
source_filename: chloris-geospatial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chloris.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 18:32:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chloris.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chloris-geospatial/refs/heads/main/security/chloris-geospatial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Geospatial
- Carbon
- Data
- Environmental
---
