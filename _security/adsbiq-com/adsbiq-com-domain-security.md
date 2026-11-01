---
api_specs:
- filename: adsbiq-com-aircraft-api-openapi.yml
  format: yaml
  label: adsbiq-com Aircraft API
  slug: adsbiq-com-aircraft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-aircraft-api-openapi.yml
- filename: adsbiq-com-airports-api-openapi.yml
  format: yaml
  label: adsbiq-com Airports API
  slug: adsbiq-com-airports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-airports-api-openapi.yml
- filename: adsbiq-com-flights-api-openapi.yml
  format: yaml
  label: adsbiq-com Flights API
  slug: adsbiq-com-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-flights-api-openapi.yml
- filename: adsbiq-com-geographic-api-openapi.yml
  format: yaml
  label: adsbiq-com Geographic API
  slug: adsbiq-com-geographic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-geographic-api-openapi.yml
- filename: adsbiq-com-network-api-openapi.yml
  format: yaml
  label: adsbiq-com Network API
  slug: adsbiq-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adsbiq-com/openapi/adsbiq-com-network-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adsbiq.com
  spf: true
hosts:
- cert_expires: Dec 14 03:46:19 2026 GMT
  host: adsbiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adsbiq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adsbiq-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: adsbiq-com
provider_slug: adsbiq-com
slug: adsbiq-com-domain-security
source_filename: adsbiq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsbiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 03:46:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adsbiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adsbiq-com/security/adsbiq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- DataAnalytics
- MarketingTechnology
- API
- Company
---
