---
api_specs:
- filename: oden-technologies-dashboards-api-openapi.yml
  format: yaml
  label: Oden Technologies Dashboards API
  slug: oden-technologies-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-dashboards-api-openapi.yml
- filename: oden-technologies-intervals-api-openapi.yml
  format: yaml
  label: Oden Technologies Intervals API
  slug: oden-technologies-intervals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-intervals-api-openapi.yml
- filename: oden-technologies-machine-groups-api-openapi.yml
  format: yaml
  label: Oden Technologies Machine Groups API
  slug: oden-technologies-machine-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-machine-groups-api-openapi.yml
- filename: oden-technologies-maintenance-work-orders-api-openapi.yml
  format: yaml
  label: Oden Technologies Maintenance Work Orders API
  slug: oden-technologies-maintenance-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-maintenance-work-orders-api-openapi.yml
- filename: oden-technologies-metric-groups-api-openapi.yml
  format: yaml
  label: Oden Technologies Metric Groups API
  slug: oden-technologies-metric-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-metric-groups-api-openapi.yml
- filename: oden-technologies-oql-api-openapi.yml
  format: yaml
  label: Oden Technologies OQL API
  slug: oden-technologies-oql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-oql-api-openapi.yml
- filename: oden-technologies-product-attributes-api-openapi.yml
  format: yaml
  label: Oden Technologies Product Attributes API
  slug: oden-technologies-product-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-product-attributes-api-openapi.yml
- filename: oden-technologies-product-mappings-api-openapi.yml
  format: yaml
  label: Oden Technologies Product Mappings API
  slug: oden-technologies-product-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-product-mappings-api-openapi.yml
- filename: oden-technologies-products-api-openapi.yml
  format: yaml
  label: Oden Technologies Products API
  slug: oden-technologies-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-products-api-openapi.yml
- filename: oden-technologies-quality-test-api-openapi.yml
  format: yaml
  label: Oden Technologies Quality Test API
  slug: oden-technologies-quality-test-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-quality-test-api-openapi.yml
- filename: oden-technologies-scrap-yield-data-api-openapi.yml
  format: yaml
  label: Oden Technologies Scrap/Yield Data API
  slug: oden-technologies-scrap-yield-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-scrap-yield-data-api-openapi.yml
- filename: oden-technologies-targets-api-openapi.yml
  format: yaml
  label: Oden Technologies Targets API
  slug: oden-technologies-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/openapi/oden-technologies-targets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "certificatemanager.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oden.io
  spf: true
- caa:
  - 0 issue "certificatemanager.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: oden.app
  spf: false
hosts:
- cert_expires: Sep 10 01:59:20 2026 GMT
  host: oden.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:53:39 2026 GMT
  host: api.oden.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oden Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oden Technologies, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oden Technologies
provider_slug: oden-technologies
slug: oden-technologies-domain-security
source_filename: oden-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oden.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:59:20 2026 GMT\n  hsts: false\n- host: api.oden.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:53:39 2026 GMT\n  hsts: null\ndomains:\n- domain: oden.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"certificatemanager.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oden.app\n  dnssec: false\n  caa:\n  - 0 issue \"certificatemanager.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oden-technologies/refs/heads/main/security/oden-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Manufacturing
- Industrial IoT
- Analytics
- Artificial Intelligence
- Factory
- Manufacturing Analytics
- API
---
