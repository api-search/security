---
api_specs:
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Companies API
  slug: simpro-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Customers API
  slug: simpro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Sites API
  slug: simpro-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Jobs API
  slug: simpro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Quotes API
  slug: simpro-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Invoices API
  slug: simpro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Schedules API
  slug: simpro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Vendor Orders API
  slug: simpro-vendor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Cost Centers API
  slug: simpro-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Stock API
  slug: simpro-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Webhooks API
  slug: simpro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simprogroup.com
  spf: true
  spf_policy: ~all
- caa: []
  dmarc: not_probed
  dnssec: false
  domain: simprosuite.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Sep 24 06:29:55 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: simprogroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 06:29:55 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: developer.simprogroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: simprosuite.com
  https: true
  note: Per-build API host parent domain; apex resolves via regional load balancers (au-lb.simprosuite.com). Individual builds are {build}.simprosuite.com.
kind: domain-security
layout: security
method: probed
name: Simpro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simpro, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Simpro
provider_slug: simpro
slug: simpro-domain-security
source_filename: simpro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + documentation hosts\nnotes: >-\n  The API itself is served per-build at https://{build}.simprosuite.com, so\n  there is no single global API host to probe. simprosuite.com is the parent\n  domain for customer build subdomains; the apex has no direct A record and\n  resolves through regional load balancers (e.g. au-lb.simprosuite.com). The\n  hosts probed below are the public website and developer/documentation hosts\n  referenced in apis.yml, both fronted by Cloudflare.\nhosts:\n- host: simprogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 24 06:29:55 2026 GMT\n  hsts: false\n- host: developer.simprogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Sep 24 06:29:55 2026 GMT\n  hsts: false\n- host: simprosuite.com\n  https: true\n  note: Per-build API host parent domain;\
  \ apex resolves via regional load balancers (au-lb.simprosuite.com). Individual builds are {build}.simprosuite.com.\ndomains:\n- domain: simprogroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: simprosuite.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: not_probed\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/security/simpro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Field Service Management
- Trades
- Job Management
- Project Management
- Scheduling
- Inventory
- Estimating
- Workforce
- SaaS
- Contractors
---
