---
api_specs:
- filename: national-highway-traffic-safety-administration-openapi.yml
  format: yaml
  label: NHTSA vPIC Vehicle API
  slug: vehicle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-highway-traffic-safety-administration/refs/heads/main/openapi/national-highway-traffic-safety-administration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nhtsa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.nhtsa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: vpic.nhtsa.dot.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Highway Traffic Safety Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Highway Traffic Safety Administration, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Highway Traffic Safety Administration
provider_slug: national-highway-traffic-safety-administration
slug: national-highway-traffic-safety-administration-domain-security
source_filename: national-highway-traffic-safety-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nhtsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: vpic.nhtsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nhtsa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-highway-traffic-safety-administration/refs/heads/main/security/national-highway-traffic-safety-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Safety
- Transportation
- Vehicles
---
