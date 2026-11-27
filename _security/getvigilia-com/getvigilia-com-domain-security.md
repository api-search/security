---
api_specs:
- filename: getvigilia-com-account-api-openapi.yml
  format: yaml
  label: Vigilia Account API
  slug: getvigilia-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-account-api-openapi.yml
- filename: getvigilia-com-apps-api-openapi.yml
  format: yaml
  label: Vigilia Apps API
  slug: getvigilia-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-apps-api-openapi.yml
- filename: getvigilia-com-errors-api-openapi.yml
  format: yaml
  label: Vigilia Errors API
  slug: getvigilia-com-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-errors-api-openapi.yml
- filename: getvigilia-com-incidents-api-openapi.yml
  format: yaml
  label: Vigilia Incidents API
  slug: getvigilia-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getvigilia-com/openapi/getvigilia-com-incidents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getvigilia.com
  spf: true
hosts:
- cert_expires: Jan  4 04:04:18 2027 GMT
  host: getvigilia.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vigilia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vigilia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vigilia
provider_slug: getvigilia-com
slug: getvigilia-com-domain-security
source_filename: getvigilia-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getvigilia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 04:04:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: getvigilia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getvigilia-com/security/getvigilia-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Monitoring
- DevOps
- Observability
- Company
---
