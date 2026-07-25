---
api_specs:
- filename: opsramp-alerts-api-openapi.yml
  format: yaml
  label: OpsRamp Alerts API
  slug: opsramp-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-alerts-api-openapi.yml
- filename: opsramp-alerts-search-api-openapi.yml
  format: yaml
  label: OpsRamp Alerts Search API
  slug: opsramp-alerts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-alerts-search-api-openapi.yml
- filename: opsramp-jobs-api-openapi.yml
  format: yaml
  label: OpsRamp Jobs API
  slug: opsramp-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-jobs-api-openapi.yml
- filename: opsramp-monitoring-api-openapi.yml
  format: yaml
  label: OpsRamp Monitoring API
  slug: opsramp-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-monitoring-api-openapi.yml
- filename: opsramp-resourcemonitors-api-openapi.yml
  format: yaml
  label: OpsRamp Resourcemonitors API
  slug: opsramp-resourcemonitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-resourcemonitors-api-openapi.yml
- filename: opsramp-resources-api-openapi.yml
  format: yaml
  label: OpsRamp Resources API
  slug: opsramp-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-resources-api-openapi.yml
- filename: opsramp-resources-search-api-openapi.yml
  format: yaml
  label: OpsRamp Resources Search API
  slug: opsramp-resources-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-resources-search-api-openapi.yml
- filename: opsramp-tenancy-api-openapi.yml
  format: yaml
  label: OpsRamp Tenancy API
  slug: opsramp-tenancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-tenancy-api-openapi.yml
- filename: opsramp-ticketentity-api-openapi.yml
  format: yaml
  label: OpsRamp Ticketentity API
  slug: opsramp-ticketentity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-ticketentity-api-openapi.yml
- filename: opsramp-ticketentity-search-api-openapi.yml
  format: yaml
  label: OpsRamp Ticketentity Search API
  slug: opsramp-ticketentity-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/openapi/opsramp-ticketentity-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "rapidssl.com"
  - 0 issue ";"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opsramp.com
  spf: true
hosts:
- cert_expires: Oct  2 04:17:34 2026 GMT
  host: www.opsramp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: api.opsramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opsramp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpsRamp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpsRamp
provider_slug: opsramp
slug: opsramp-domain-security
source_filename: opsramp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opsramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:17:34 2026 GMT\n  hsts: null\n- host: api.opsramp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opsramp.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"rapidssl.com\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opsramp/refs/heads/main/security/opsramp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIOps
- IT Operations
---
