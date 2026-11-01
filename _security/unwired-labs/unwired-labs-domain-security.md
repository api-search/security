---
api_specs:
- filename: unwired-labs-balance-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) BALANCE API
  slug: unwired-labs-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-balance-api-openapi.yml
- filename: unwired-labs-geolocation-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) GEOLOCATION API
  slug: unwired-labs-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-geolocation-api-openapi.yml
- filename: unwired-labs-reverse-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) REVERSE API
  slug: unwired-labs-reverse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-reverse-api-openapi.yml
- filename: unwired-labs-search-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) SEARCH API
  slug: unwired-labs-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-search-api-openapi.yml
- filename: unwired-labs-timezone-api-openapi.yml
  format: yaml
  label: Unwired Labs (incl. OpenCelliD) Timezone API
  slug: unwired-labs-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unwired-labs/openapi/unwired-labs-timezone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unwiredlabs.com
  spf: true
hosts:
- cert_expires: Jan  3 21:29:21 2027 GMT
  host: unwiredlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unwired Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unwired Labs (incl. OpenCelliD), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unwired Labs (incl. OpenCelliD)
provider_slug: unwired-labs
slug: unwired-labs-domain-security
source_filename: unwired-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unwiredlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:29:21 2027 GMT\n  hsts: false\ndomains:\n- domain: unwiredlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/unwired-labs/security/unwired-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Location API
- Geolocation
- Mapping
- OpenCelliD
---
