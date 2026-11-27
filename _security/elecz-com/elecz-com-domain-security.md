---
api_specs:
- filename: elecz-com-go-api-openapi.yml
  format: yaml
  label: Elecz Go API
  slug: elecz-com-go-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elecz-com/openapi/elecz-com-go-api-openapi.yml
- filename: elecz-com-health-api-openapi.yml
  format: yaml
  label: Elecz Health API
  slug: elecz-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elecz-com/openapi/elecz-com-health-api-openapi.yml
- filename: elecz-com-signal-api-openapi.yml
  format: yaml
  label: Elecz Signal API
  slug: elecz-com-signal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elecz-com/openapi/elecz-com-signal-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elecz.com
  spf: true
hosts:
- cert_expires: Jan 18 17:21:30 2027 GMT
  host: elecz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elecz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elecz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Elecz
provider_slug: elecz-com
slug: elecz-com-domain-security
source_filename: elecz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elecz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 17:21:30 2027 GMT\n  hsts: false\ndomains:\n- domain: elecz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/elecz-com/security/elecz-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Artificial Intelligence
- Electricity
- Pricing
- Comparison
---
