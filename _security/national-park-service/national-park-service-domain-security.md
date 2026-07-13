---
api_specs:
- filename: national-park-service-openapi.yml
  format: yaml
  label: National Park Service API
  slug: national-park-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/openapi/national-park-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nps.gov
  spf: true
hosts:
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
name: National Park Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Park Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Park Service
provider_slug: national-park-service
slug: national-park-service-domain-security
source_filename: national-park-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nps.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:20:55 2026 GMT\n  hsts: null\ndomains:\n- domain: nps.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-park-service/refs/heads/main/security/national-park-service-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Conservation
- Federal Government
- Parks
---
