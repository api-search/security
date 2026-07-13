---
api_specs:
- filename: usgs-earthquake-api-openapi.yaml
  format: yaml
  label: Earthquake Notifications, Feeds, and Web Services
  slug: earthquake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/openapi/usgs-earthquake-api-openapi.yaml
- filename: usgs-water-data-api-openapi.yaml
  format: yaml
  label: USGS Water Data APIs
  slug: water-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/openapi/usgs-water-data-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usgs.gov
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: www.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: earthquake.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 21:20:52 2026 GMT
  host: api.waterdata.usgs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: U S Geological Survey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Geological Survey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Geological Survey
provider_slug: u-s-geological-survey
slug: u-s-geological-survey-domain-security
source_filename: u-s-geological-survey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: earthquake.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.waterdata.usgs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:20:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usgs.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-geological-survey/refs/heads/main/security/u-s-geological-survey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Geological
- Earth Science
- Natural Resources
- Earthquake
- Water
- Hydrology
---
