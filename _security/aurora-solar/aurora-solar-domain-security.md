---
api_specs:
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Projects API
  slug: aurora-solar-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Designs API
  slug: aurora-solar-designs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Proposals API
  slug: aurora-solar-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Consumption Profiles API
  slug: aurora-solar-consumption-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Users & Tenants API
  slug: aurora-solar-users-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Webhooks API
  slug: aurora-solar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Financings API
  slug: aurora-solar-financings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
- filename: aurora-solar-openapi.yml
  format: yaml
  label: Aurora Solar Agreements API
  slug: aurora-solar-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/openapi/aurora-solar-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aurorasolar.com
  spf: true
hosts:
- cert_expires: Aug 15 01:24:40 2026 GMT
  host: aurorasolar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 11:11:13 2026 GMT
  host: docs.aurorasolar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.aurorasolar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurora Solar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora Solar, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aurora Solar
provider_slug: aurora-solar
slug: aurora-solar-domain-security
source_filename: aurora-solar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurorasolar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 01:24:40 2026 GMT\n  hsts: false\n- host: docs.aurorasolar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 11:11:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aurorasolar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aurorasolar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-solar/refs/heads/main/security/aurora-solar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solar
- Solar Design
- PV
- Proposals
- CleanTech
- Energy
- Sales Software
---
