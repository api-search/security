---
api_specs:
- filename: launchflag-dev-evaluation-api-openapi.yml
  format: yaml
  label: LaunchFlag Evaluation API
  slug: launchflag-dev-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-evaluation-api-openapi.yml
- filename: launchflag-dev-management-api-openapi.yml
  format: yaml
  label: LaunchFlag Management API
  slug: launchflag-dev-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-management-api-openapi.yml
- filename: launchflag-dev-meta-api-openapi.yml
  format: yaml
  label: LaunchFlag Meta API
  slug: launchflag-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchflag-dev/openapi/launchflag-dev-meta-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: launchflag.dev
  spf: true
hosts:
- cert_expires: Jan 31 17:32:12 2027 GMT
  host: launchflag.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LaunchFlag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LaunchFlag, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LaunchFlag
provider_slug: launchflag-dev
slug: launchflag-dev-domain-security
source_filename: launchflag-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launchflag.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 17:32:12 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: launchflag.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/launchflag-dev/security/launchflag-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Feature Flags
- Kill Switch
- Rollouts
- Targeting
- Audit Logs
- SDK
---
