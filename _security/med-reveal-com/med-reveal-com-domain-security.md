---
api_specs:
- filename: med-reveal-com-benchmarking-api-api-openapi.yml
  format: yaml
  label: MedReveal Benchmarking API
  slug: med-reveal-com-benchmarking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-benchmarking-api-api-openapi.yml
- filename: med-reveal-com-health-api-openapi.yml
  format: yaml
  label: MedReveal Health API
  slug: med-reveal-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-health-api-openapi.yml
- filename: med-reveal-com-market-api-api-openapi.yml
  format: yaml
  label: MedReveal Market API
  slug: med-reveal-com-market-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-market-api-api-openapi.yml
- filename: med-reveal-com-npi-api-api-openapi.yml
  format: yaml
  label: MedReveal Npi API
  slug: med-reveal-com-npi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-npi-api-api-openapi.yml
- filename: med-reveal-com-provider-api-api-openapi.yml
  format: yaml
  label: MedReveal Provider API
  slug: med-reveal-com-provider-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-provider-api-api-openapi.yml
- filename: med-reveal-com-taxonomy-api-api-openapi.yml
  format: yaml
  label: MedReveal Taxonomy API
  slug: med-reveal-com-taxonomy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-taxonomy-api-api-openapi.yml
- filename: med-reveal-com-tin-api-api-openapi.yml
  format: yaml
  label: MedReveal Tin API
  slug: med-reveal-com-tin-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-tin-api-api-openapi.yml
- filename: med-reveal-com-usage-api-api-openapi.yml
  format: yaml
  label: MedReveal Usage API
  slug: med-reveal-com-usage-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/med-reveal-com/openapi/med-reveal-com-usage-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: med-reveal.com
  spf: true
hosts:
- cert_expires: Apr 28 23:59:59 2027 GMT
  host: www.med-reveal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MedReveal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedReveal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MedReveal
provider_slug: med-reveal-com
slug: med-reveal-com-domain-security
source_filename: med-reveal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.med-reveal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: med-reveal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/med-reveal-com/security/med-reveal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pricing
- Data Analytics
- MCP
---
