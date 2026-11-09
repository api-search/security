---
api_specs:
- filename: backresto-com-agent-api-openapi.yml
  format: yaml
  label: BackResto Agent API
  slug: backresto-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-agent-api-openapi.yml
- filename: backresto-com-allergens-api-openapi.yml
  format: yaml
  label: BackResto Allergens API
  slug: backresto-com-allergens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-allergens-api-openapi.yml
- filename: backresto-com-audit-api-openapi.yml
  format: yaml
  label: BackResto Audit API
  slug: backresto-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-audit-api-openapi.yml
- filename: backresto-com-health-api-openapi.yml
  format: yaml
  label: BackResto Health API
  slug: backresto-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-health-api-openapi.yml
- filename: backresto-com-meta-api-openapi.yml
  format: yaml
  label: BackResto Meta API
  slug: backresto-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-meta-api-openapi.yml
- filename: backresto-com-mobile-api-openapi.yml
  format: yaml
  label: BackResto Mobile API
  slug: backresto-com-mobile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-mobile-api-openapi.yml
- filename: backresto-com-module-assets-api-openapi.yml
  format: yaml
  label: BackResto module assets API
  slug: backresto-com-module-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-module-assets-api-openapi.yml
- filename: backresto-com-module-shadow-ingestion-api-openapi.yml
  format: yaml
  label: BackResto module shadow ingestion API
  slug: backresto-com-module-shadow-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-module-shadow-ingestion-api-openapi.yml
- filename: backresto-com-partner-restaurants-api-openapi.yml
  format: yaml
  label: BackResto partner restaurants API
  slug: backresto-com-partner-restaurants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-partner-restaurants-api-openapi.yml
- filename: backresto-com-received-module-snapshots-api-openapi.yml
  format: yaml
  label: BackResto received module snapshots API
  slug: backresto-com-received-module-snapshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/backresto-com/openapi/backresto-com-received-module-snapshots-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: backresto.com
  spf: true
hosts:
- cert_expires: Jan  4 03:07:41 2027 GMT
  host: backresto.com
  hsts: true
  hsts_max_age: 31104000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Backresto Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BackResto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BackResto
provider_slug: backresto-com
slug: backresto-com-domain-security
source_filename: backresto-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backresto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 03:07:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31104000\ndomains:\n- domain: backresto.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/backresto-com/security/backresto-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food
- Restaurant
- HACCP
- Compliance
- Safety
- French
---
