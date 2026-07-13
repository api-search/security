---
api_specs:
- filename: regrid-parcel-openapi.yml
  format: yaml
  label: Regrid Parcel API
  slug: regrid-parcel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/openapi/regrid-parcel-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: regrid.com
  spf: true
hosts:
- cert_expires: Aug 30 11:00:01 2026 GMT
  host: regrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:04:59 2026 GMT
  host: app.regrid.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Regrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regrid, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Regrid
provider_slug: regrid
slug: regrid-domain-security
source_filename: regrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.regrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:04:59 2026 GMT\n  hsts: false\ndomains:\n- domain: regrid.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regrid/refs/heads/main/security/regrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Parcels
- Land Data
- Property Data
- GeoJSON
- Real Estate
- Zoning
- Ownership
- Geospatial
- Mapping
- Tiles
---
