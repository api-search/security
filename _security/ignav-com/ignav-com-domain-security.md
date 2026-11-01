---
api_specs:
- filename: ignav-com-airports-api-openapi.yml
  format: yaml
  label: ignav-com Airports API
  slug: ignav-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-airports-api-openapi.yml
- filename: ignav-com-fares-api-openapi.yml
  format: yaml
  label: ignav-com Fares API
  slug: ignav-com-fares-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-fares-api-openapi.yml
- filename: ignav-com-health-api-openapi.yml
  format: yaml
  label: ignav-com Health API
  slug: ignav-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ignav-com/openapi/ignav-com-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ignav.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: ignav.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ignav Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ignav-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ignav-com
provider_slug: ignav-com
slug: ignav-com-domain-security
source_filename: ignav-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ignav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ignav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ignav-com/security/ignav-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Flight
- Travel
- API
- Pricing
- Data
---
