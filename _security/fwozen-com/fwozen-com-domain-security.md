---
api_specs:
- filename: fwozen-com-api-keys-api-openapi.yml
  format: yaml
  label: Fwozen API keys API
  slug: fwozen-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-api-keys-api-openapi.yml
- filename: fwozen-com-audit-api-openapi.yml
  format: yaml
  label: Fwozen Audit API
  slug: fwozen-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-audit-api-openapi.yml
- filename: fwozen-com-billing-api-openapi.yml
  format: yaml
  label: Fwozen Billing API
  slug: fwozen-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-billing-api-openapi.yml
- filename: fwozen-com-branches-api-openapi.yml
  format: yaml
  label: Fwozen Branches API
  slug: fwozen-com-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-branches-api-openapi.yml
- filename: fwozen-com-enforcement-api-openapi.yml
  format: yaml
  label: Fwozen Enforcement API
  slug: fwozen-com-enforcement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-enforcement-api-openapi.yml
- filename: fwozen-com-exceptions-api-openapi.yml
  format: yaml
  label: Fwozen Exceptions API
  slug: fwozen-com-exceptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-exceptions-api-openapi.yml
- filename: fwozen-com-freezes-api-openapi.yml
  format: yaml
  label: Fwozen Freezes API
  slug: fwozen-com-freezes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-freezes-api-openapi.yml
- filename: fwozen-com-organizations-api-openapi.yml
  format: yaml
  label: Fwozen Organizations API
  slug: fwozen-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-organizations-api-openapi.yml
- filename: fwozen-com-repositories-api-openapi.yml
  format: yaml
  label: Fwozen Repositories API
  slug: fwozen-com-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-repositories-api-openapi.yml
- filename: fwozen-com-schedules-api-openapi.yml
  format: yaml
  label: Fwozen Schedules API
  slug: fwozen-com-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fwozen-com/openapi/fwozen-com-schedules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fwozen.com
  spf: true
hosts:
- cert_expires: Dec 26 20:33:15 2026 GMT
  host: fwozen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fwozen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fwozen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fwozen
provider_slug: fwozen-com
slug: fwozen-com-domain-security
source_filename: fwozen-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fwozen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:33:15 2026 GMT\n  hsts: false\ndomains:\n- domain: fwozen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fwozen-com/security/fwozen-com-domain-security.yml
summary_line: TLSv1.3
tags:
- GitHub
- code freeze
- merge freeze
- deploy gate
- Security
---
