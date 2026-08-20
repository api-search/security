---
api_specs:
- filename: department-of-the-interior-alerts-api-openapi.yml
  format: yaml
  label: Department of the Interior Alerts API
  slug: department-of-the-interior-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-alerts-api-openapi.yml
- filename: department-of-the-interior-articles-api-openapi.yml
  format: yaml
  label: Department of the Interior Articles API
  slug: department-of-the-interior-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-articles-api-openapi.yml
- filename: department-of-the-interior-campgrounds-api-openapi.yml
  format: yaml
  label: Department of the Interior Campgrounds API
  slug: department-of-the-interior-campgrounds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-campgrounds-api-openapi.yml
- filename: department-of-the-interior-counts-api-openapi.yml
  format: yaml
  label: Department of the Interior Counts API
  slug: department-of-the-interior-counts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-counts-api-openapi.yml
- filename: department-of-the-interior-dailyvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior DailyValues API
  slug: department-of-the-interior-dailyvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-dailyvalues-api-openapi.yml
- filename: department-of-the-interior-events-api-openapi.yml
  format: yaml
  label: Department of the Interior Events API
  slug: department-of-the-interior-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-events-api-openapi.yml
- filename: department-of-the-interior-instantaneousvalues-api-openapi.yml
  format: yaml
  label: Department of the Interior InstantaneousValues API
  slug: department-of-the-interior-instantaneousvalues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-instantaneousvalues-api-openapi.yml
- filename: department-of-the-interior-parks-api-openapi.yml
  format: yaml
  label: Department of the Interior Parks API
  slug: department-of-the-interior-parks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-parks-api-openapi.yml
- filename: department-of-the-interior-sites-api-openapi.yml
  format: yaml
  label: Department of the Interior Sites API
  slug: department-of-the-interior-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-sites-api-openapi.yml
- filename: department-of-the-interior-visitorcenters-api-openapi.yml
  format: yaml
  label: Department of the Interior VisitorCenters API
  slug: department-of-the-interior-visitorcenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/openapi/department-of-the-interior-visitorcenters-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: doi.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nps.gov
  spf: true
hosts:
- cert_expires: Oct  8 17:48:45 2026 GMT
  host: www.doi.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.nps.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 17:20:55 2026 GMT
  host: developer.nps.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of The Interior Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of the Interior, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of the Interior
provider_slug: department-of-the-interior
slug: department-of-the-interior-domain-security
source_filename: department-of-the-interior-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doi.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: doi.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nps.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-the-interior/refs/heads/main/security/department-of-the-interior-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal-Government
- Public Lands
- Natural Resources
- Geospatial
---
