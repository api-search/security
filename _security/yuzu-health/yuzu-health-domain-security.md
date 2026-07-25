---
api_specs:
- filename: yuzu-health-accumulator-experimental-api-openapi.yml
  format: yaml
  label: Yuzu Health Accumulator (Experimental) API
  slug: yuzu-health-accumulator-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-accumulator-experimental-api-openapi.yml
- filename: yuzu-health-benefits-api-openapi.yml
  format: yaml
  label: Yuzu Health Benefits API
  slug: yuzu-health-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-benefits-api-openapi.yml
- filename: yuzu-health-coverage-api-openapi.yml
  format: yaml
  label: Yuzu Health Coverage API
  slug: yuzu-health-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-coverage-api-openapi.yml
- filename: yuzu-health-enrollment-api-openapi.yml
  format: yaml
  label: Yuzu Health Enrollment API
  slug: yuzu-health-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-enrollment-api-openapi.yml
- filename: yuzu-health-eob-experimental-api-openapi.yml
  format: yaml
  label: Yuzu Health EOB (Experimental) API
  slug: yuzu-health-eob-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-eob-experimental-api-openapi.yml
- filename: yuzu-health-group-policy-api-openapi.yml
  format: yaml
  label: Yuzu Health Group Policy API
  slug: yuzu-health-group-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-group-policy-api-openapi.yml
- filename: yuzu-health-member-api-openapi.yml
  format: yaml
  label: Yuzu Health Member API
  slug: yuzu-health-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-member-api-openapi.yml
- filename: yuzu-health-publicapiv1-api-openapi.yml
  format: yaml
  label: Yuzu Health PublicApiV1 API
  slug: yuzu-health-publicapiv1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-publicapiv1-api-openapi.yml
- filename: yuzu-health-publicapiv2-api-openapi.yml
  format: yaml
  label: Yuzu Health PublicApiV2 API
  slug: yuzu-health-publicapiv2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-publicapiv2-api-openapi.yml
- filename: yuzu-health-sponsor-api-openapi.yml
  format: yaml
  label: Yuzu Health Sponsor API
  slug: yuzu-health-sponsor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/openapi/yuzu-health-sponsor-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yuzu.health
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: yuzu.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yuzu Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuzu Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yuzu Health
provider_slug: yuzu-health
slug: yuzu-health-domain-security
source_filename: yuzu-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yuzu.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yuzu.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuzu-health/refs/heads/main/security/yuzu-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Insurance
- Health Plans
- Benefits Administration
- Claims
- Enrollment
- Payers
- Self-Funded
---
