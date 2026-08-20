---
api_specs:
- filename: optscale-authentication-api-openapi.yml
  format: yaml
  label: OptScale Authentication API
  slug: optscale-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-authentication-api-openapi.yml
- filename: optscale-cloud-accounts-api-openapi.yml
  format: yaml
  label: OptScale Cloud Accounts API
  slug: optscale-cloud-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-cloud-accounts-api-openapi.yml
- filename: optscale-employees-api-openapi.yml
  format: yaml
  label: OptScale Employees API
  slug: optscale-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-employees-api-openapi.yml
- filename: optscale-expenses-api-openapi.yml
  format: yaml
  label: OptScale Expenses API
  slug: optscale-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-expenses-api-openapi.yml
- filename: optscale-optimizations-api-openapi.yml
  format: yaml
  label: OptScale Optimizations API
  slug: optscale-optimizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-optimizations-api-openapi.yml
- filename: optscale-organizations-api-openapi.yml
  format: yaml
  label: OptScale Organizations API
  slug: optscale-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-organizations-api-openapi.yml
- filename: optscale-pools-api-openapi.yml
  format: yaml
  label: OptScale Pools API
  slug: optscale-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-pools-api-openapi.yml
- filename: optscale-recommendations-api-openapi.yml
  format: yaml
  label: OptScale Recommendations API
  slug: optscale-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-recommendations-api-openapi.yml
- filename: optscale-resources-api-openapi.yml
  format: yaml
  label: OptScale Resources API
  slug: optscale-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/openapi/optscale-resources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hystax.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: optscale.com
  spf: true
hosts:
- cert_expires: Sep  7 21:58:09 2026 GMT
  host: hystax.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 18:17:08 2026 GMT
  host: my.optscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OptScale, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OptScale
provider_slug: optscale
slug: optscale-domain-security
source_filename: optscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hystax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:58:09 2026 GMT\n  hsts: false\n- host: my.optscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 18:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hystax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: optscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optscale/refs/heads/main/security/optscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinOps
- Cost Optimization
- Cloud
- Kubernetes
- Open-Source
---
