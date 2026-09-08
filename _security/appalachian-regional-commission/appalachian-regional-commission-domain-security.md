---
api_specs:
- filename: appalachian-regional-commission-research-api-openapi.yml
  format: yaml
  label: ARC Research and Data API
  slug: arc-research-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-research-api-openapi.yml
- filename: appalachian-regional-commission-geospatial-api-openapi.yml
  format: yaml
  label: ARC Geospatial API
  slug: arc-geospatial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-geospatial-api-openapi.yml
- filename: appalachian-regional-commission-programs-api-openapi.yml
  format: yaml
  label: ARC Programs API
  slug: arc-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-programs-api-openapi.yml
- filename: appalachian-regional-commission-content-api-openapi.yml
  format: yaml
  label: ARC Content API
  slug: arc-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-content-api-openapi.yml
- filename: appalachian-regional-commission-taxonomy-api-openapi.yml
  format: yaml
  label: ARC Taxonomy API
  slug: arc-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-taxonomy-api-openapi.yml
- filename: appalachian-regional-commission-discovery-api-openapi.yml
  format: yaml
  label: ARC API Discovery
  slug: arc-api-discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arc.gov
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arcgis.com
  spf: true
hosts:
- cert_expires: Oct 15 08:23:34 2026 GMT
  host: www.arc.gov
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 02:18:33 2026 GMT
  host: data.arc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Appalachian Regional Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appalachian Regional Commission, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Appalachian Regional Commission
provider_slug: appalachian-regional-commission
slug: appalachian-regional-commission-domain-security
source_filename: appalachian-regional-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 08:23:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: data.arc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 02:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arc.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: arcgis.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/security/appalachian-regional-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Appalachia
- Economic Development
- Federal-Government
- Geospatial
- Government
- Infrastructure
- Open Data
- Regional Development
- Workforce Development
---
