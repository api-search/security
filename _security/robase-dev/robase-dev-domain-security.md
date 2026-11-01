---
api_specs:
- filename: robase-dev-dashboard-api-openapi.yml
  format: yaml
  label: robase-dev Dashboard API
  slug: robase-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-dashboard-api-openapi.yml
- filename: robase-dev-otp-api-openapi.yml
  format: yaml
  label: robase-dev OTP API
  slug: robase-dev-otp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-otp-api-openapi.yml
- filename: robase-dev-sms-api-openapi.yml
  format: yaml
  label: robase-dev SMS API
  slug: robase-dev-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-sms-api-openapi.yml
- filename: robase-dev-system-api-openapi.yml
  format: yaml
  label: robase-dev System API
  slug: robase-dev-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/robase-dev/openapi/robase-dev-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: robase.dev
  spf: true
hosts:
- cert_expires: Jan  9 20:31:27 2027 GMT
  host: robase.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Robase Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for robase-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: robase-dev
provider_slug: robase-dev
slug: robase-dev-domain-security
source_filename: robase-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: robase.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 20:31:27 2027 GMT\n  hsts: false\ndomains:\n- domain: robase.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/robase-dev/security/robase-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- SMS
- OTP
- Africa
- Messaging
- API
- Communications
---
