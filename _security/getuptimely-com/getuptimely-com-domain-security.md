---
api_specs:
- filename: getuptimely-com-alerts-api-openapi.yml
  format: yaml
  label: Uptimely Alerts API
  slug: getuptimely-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-alerts-api-openapi.yml
- filename: getuptimely-com-incidents-api-openapi.yml
  format: yaml
  label: Uptimely Incidents API
  slug: getuptimely-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-incidents-api-openapi.yml
- filename: getuptimely-com-monitors-api-openapi.yml
  format: yaml
  label: Uptimely Monitors API
  slug: getuptimely-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-monitors-api-openapi.yml
- filename: getuptimely-com-on-call-api-openapi.yml
  format: yaml
  label: Uptimely On Call API
  slug: getuptimely-com-on-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-on-call-api-openapi.yml
- filename: getuptimely-com-scheduled-maintenances-api-openapi.yml
  format: yaml
  label: Uptimely Scheduled Maintenances API
  slug: getuptimely-com-scheduled-maintenances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-scheduled-maintenances-api-openapi.yml
- filename: getuptimely-com-status-pages-api-openapi.yml
  format: yaml
  label: Uptimely Status Pages API
  slug: getuptimely-com-status-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-status-pages-api-openapi.yml
- filename: getuptimely-com-usage-api-openapi.yml
  format: yaml
  label: Uptimely Usage API
  slug: getuptimely-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-usage-api-openapi.yml
- filename: getuptimely-com-webhooks-api-openapi.yml
  format: yaml
  label: Uptimely Webhooks API
  slug: getuptimely-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getuptimely-com/openapi/getuptimely-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getuptimely.com
  spf: false
hosts:
- cert_expires: Jan 21 07:46:42 2027 GMT
  host: getuptimely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uptimely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uptimely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Uptimely
provider_slug: getuptimely-com
slug: getuptimely-com-domain-security
source_filename: getuptimely-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getuptimely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 07:46:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getuptimely.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getuptimely-com/security/getuptimely-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Uptime
- Status Pages
- On-Call
---
