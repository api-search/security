---
api_specs:
- filename: anthid-com-account-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Manual Controls API
  slug: anthid-com-account-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-manual-controls-api-openapi.yml
- filename: anthid-com-account-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Risk Controls API
  slug: anthid-com-account-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-risk-controls-api-openapi.yml
- filename: anthid-com-account-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Time Controls API
  slug: anthid-com-account-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-time-controls-api-openapi.yml
- filename: anthid-com-control-evaluation-api-openapi.yml
  format: yaml
  label: anthid-com Control Evaluation API
  slug: anthid-com-control-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-control-evaluation-api-openapi.yml
- filename: anthid-com-effective-controls-api-openapi.yml
  format: yaml
  label: anthid-com Effective Controls API
  slug: anthid-com-effective-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-effective-controls-api-openapi.yml
- filename: anthid-com-organization-controls-api-openapi.yml
  format: yaml
  label: anthid-com Organization Controls API
  slug: anthid-com-organization-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-organization-controls-api-openapi.yml
- filename: anthid-com-symbol-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Manual Controls API
  slug: anthid-com-symbol-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-manual-controls-api-openapi.yml
- filename: anthid-com-symbol-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Risk Controls API
  slug: anthid-com-symbol-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-risk-controls-api-openapi.yml
- filename: anthid-com-symbol-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Time Controls API
  slug: anthid-com-symbol-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-time-controls-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anthid.com
  spf: true
hosts:
- host: anthid.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anthid Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for anthid-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: anthid-com
provider_slug: anthid-com
slug: anthid-com-domain-security
source_filename: anthid-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anthid.com\n  https: false\ndomains:\n- domain: anthid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anthid-com/security/anthid-com-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
