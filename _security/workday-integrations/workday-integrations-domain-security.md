---
api_specs:
- filename: openapi.json
  format: json
  label: Workday REST API
  slug: workday-rest-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/restapi/openapi.json
- filename: workday-integrations-raas-openapi.yml
  format: yaml
  label: Workday RaaS (Report-as-a-Service)
  slug: workday-raas-report-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-raas-openapi.yml
- filename: workday-integrations-prism-analytics-openapi.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: workday-prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/openapi/workday-integrations-prism-analytics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: doc.workday.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Integrations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Integrations, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Integrations
provider_slug: workday-integrations
slug: workday-integrations-domain-security
source_filename: workday-integrations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: doc.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/security/workday-integrations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
---
