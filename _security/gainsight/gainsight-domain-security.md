---
api_specs:
- filename: swagger
  format: yaml
  label: Gainsight REST API
  slug: gainsight-rest-api
  spec_type: OpenAPI
  url: https://api.gainsight.com/swagger
- filename: gainsight-px-api-openapi.yml
  format: yaml
  label: Gainsight PX API
  slug: gainsight-px-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-px-api-openapi.yml
- filename: gainsight-cs-company-api-openapi.yml
  format: yaml
  label: Gainsight CS Company API
  slug: gainsight-cs-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-company-api-openapi.yml
- filename: gainsight-cs-person-api-openapi.yml
  format: yaml
  label: Gainsight CS Person API
  slug: gainsight-cs-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-person-api-openapi.yml
- filename: gainsight-cs-custom-object-api-openapi.yml
  format: yaml
  label: Gainsight CS Custom Object API
  slug: gainsight-cs-custom-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-custom-object-api-openapi.yml
- filename: gainsight-cs-cta-api-openapi.yml
  format: yaml
  label: Gainsight CS CTA API
  slug: gainsight-cs-cta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-cta-api-openapi.yml
- filename: gainsight-cs-timeline-api-openapi.yml
  format: yaml
  label: Gainsight CS Timeline API
  slug: gainsight-cs-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-timeline-api-openapi.yml
- filename: gainsight-cs-success-plan-api-openapi.yml
  format: yaml
  label: Gainsight CS Success Plan API
  slug: gainsight-cs-success-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-success-plan-api-openapi.yml
- filename: gainsight-cs-data-management-api-openapi.yml
  format: yaml
  label: Gainsight CS Data Management API
  slug: gainsight-cs-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-data-management-api-openapi.yml
- filename: gainsight-cs-bulk-api-openapi.yml
  format: yaml
  label: Gainsight CS Bulk API
  slug: gainsight-cs-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-bulk-api-openapi.yml
- filename: gainsight-cs-events-api-openapi.yml
  format: yaml
  label: Gainsight CS Events API
  slug: gainsight-cs-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-events-api-openapi.yml
- filename: gainsight-cs-user-management-api-openapi.yml
  format: yaml
  label: Gainsight CS User Management API
  slug: gainsight-cs-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-user-management-api-openapi.yml
- filename: gainsight-cs-customer-goals-api-openapi.yml
  format: yaml
  label: Gainsight CS Customer Goals API
  slug: gainsight-cs-customer-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-customer-goals-api-openapi.yml
- filename: gainsight-cs-renewal-center-api-openapi.yml
  format: yaml
  label: Gainsight CS Renewal Center API
  slug: gainsight-cs-renewal-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-renewal-center-api-openapi.yml
- filename: gainsight-cs-task-and-playbook-api-openapi.yml
  format: yaml
  label: Gainsight CS Task and Playbook API
  slug: gainsight-cs-task-and-playbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/openapi/gainsight-cs-task-and-playbook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gainsight.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aptrinsic.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: support.gainsight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.gainsight.com
  https: false
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: api.aptrinsic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gainsight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gainsight, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gainsight
provider_slug: gainsight
slug: gainsight-domain-security
source_filename: gainsight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.gainsight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gainsight.com\n  https: false\n- host: api.aptrinsic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gainsight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aptrinsic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/security/gainsight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
