---
api_specs:
- filename: doi-usgs-water-openapi.yml
  format: yaml
  label: USGS Water Data APIs
  slug: usgs-water-data-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doi/refs/heads/main/openapi/doi-usgs-water-openapi.yml
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
name: Doi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Interior, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Interior
provider_slug: doi
slug: doi-domain-security
source_filename: doi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doi.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: doi.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nps.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doi/refs/heads/main/security/doi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- National Parks
- Federal Lands
- Water Resources
- Wildlife
- Minerals
- Geospatial
- Geology
- Native American Affairs
- Public Lands
---
