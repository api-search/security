---
api_specs:
- filename: helidon-health-api-openapi.yml
  format: yaml
  label: Helidon Health API
  slug: helidon-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helidon/refs/heads/main/openapi/helidon-health-api-openapi.yml
- filename: helidon-info-api-openapi.yml
  format: yaml
  label: Helidon Info API
  slug: helidon-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helidon/refs/heads/main/openapi/helidon-info-api-openapi.yml
- filename: helidon-metrics-api-openapi.yml
  format: yaml
  label: Helidon Metrics API
  slug: helidon-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helidon/refs/heads/main/openapi/helidon-metrics-api-openapi.yml
- filename: helidon-openapi-api-openapi.yml
  format: yaml
  label: Helidon OpenAPI API
  slug: helidon-openapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helidon/refs/heads/main/openapi/helidon-openapi-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helidon.io
  spf: false
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: helidon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helidon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helidon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Helidon
provider_slug: helidon
slug: helidon-domain-security
source_filename: helidon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helidon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: helidon.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helidon/refs/heads/main/security/helidon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Frameworks
- Java
- MicroProfile
- Microservices
- Oracle
- Reactive
---
