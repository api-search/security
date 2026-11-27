---
api_specs:
- filename: gisgp-com-convert-api-openapi.yml
  format: yaml
  label: GISGP Convert API
  slug: gisgp-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gisgp-com/openapi/gisgp-com-convert-api-openapi.yml
- filename: gisgp-com-tools-api-openapi.yml
  format: yaml
  label: GISGP Tools API
  slug: gisgp-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gisgp-com/openapi/gisgp-com-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gisgp.com
  spf: true
hosts:
- cert_expires: Dec 25 20:21:49 2026 GMT
  host: gisgp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GISGP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GISGP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GISGP
provider_slug: gisgp-com
slug: gisgp-com-domain-security
source_filename: gisgp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gisgp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 20:21:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gisgp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gisgp-com/security/gisgp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GIS
- Conversion
- GeoJSON
- ArcGIS
---
