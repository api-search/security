---
api_specs:
- filename: dtmframe-com-compare-api-openapi.yml
  format: yaml
  label: DTMFRAME Compare API
  slug: dtmframe-com-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-compare-api-openapi.yml
- filename: dtmframe-com-deals-api-openapi.yml
  format: yaml
  label: DTMFRAME Deals API
  slug: dtmframe-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-deals-api-openapi.yml
- filename: dtmframe-com-products-api-openapi.yml
  format: yaml
  label: DTMFRAME Products API
  slug: dtmframe-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-products-api-openapi.yml
- filename: dtmframe-com-resolve-api-openapi.yml
  format: yaml
  label: DTMFRAME Resolve API
  slug: dtmframe-com-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dtmframe-com/openapi/dtmframe-com-resolve-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dtmframe.com
  spf: true
hosts:
- cert_expires: Dec 20 21:01:00 2026 GMT
  host: dtmframe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dtmframe Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DTMFRAME, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DTMFRAME
provider_slug: dtmframe-com
slug: dtmframe-com-domain-security
source_filename: dtmframe-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dtmframe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 21:01:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dtmframe.com\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dtmframe-com/security/dtmframe-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Price-Tracking
- Japanese
- Plugins
---
