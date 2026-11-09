---
api_specs:
- filename: buildpulse-io-auth-api-openapi.yml
  format: yaml
  label: BuildPulse Auth API
  slug: buildpulse-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-auth-api-openapi.yml
- filename: buildpulse-io-badges-api-openapi.yml
  format: yaml
  label: BuildPulse Badges API
  slug: buildpulse-io-badges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-badges-api-openapi.yml
- filename: buildpulse-io-flaky-api-openapi.yml
  format: yaml
  label: BuildPulse Flaky API
  slug: buildpulse-io-flaky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-flaky-api-openapi.yml
- filename: buildpulse-io-health-api-openapi.yml
  format: yaml
  label: BuildPulse Health API
  slug: buildpulse-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-health-api-openapi.yml
- filename: buildpulse-io-submissions-api-openapi.yml
  format: yaml
  label: BuildPulse Submissions API
  slug: buildpulse-io-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-submissions-api-openapi.yml
- filename: buildpulse-io-tests-api-openapi.yml
  format: yaml
  label: BuildPulse Tests API
  slug: buildpulse-io-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-tests-api-openapi.yml
- filename: buildpulse-io-webhooks-api-openapi.yml
  format: yaml
  label: BuildPulse Webhooks API
  slug: buildpulse-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildpulse-io/openapi/buildpulse-io-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: buildpulse.io
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: buildpulse.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buildpulse Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BuildPulse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BuildPulse
provider_slug: buildpulse-io
slug: buildpulse-io-domain-security
source_filename: buildpulse-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildpulse.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildpulse.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buildpulse-io/security/buildpulse-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CI
- DevOps
- Testing
- Artificial Intelligence
- Analytics
- Company
---
