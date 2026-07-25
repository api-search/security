---
api_specs:
- filename: alteryx-collections-api-openapi.yml
  format: yaml
  label: Alteryx Collections API
  slug: alteryx-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-collections-api-openapi.yml
- filename: alteryx-credentials-api-openapi.yml
  format: yaml
  label: Alteryx Credentials API
  slug: alteryx-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-credentials-api-openapi.yml
- filename: alteryx-jobs-api-openapi.yml
  format: yaml
  label: Alteryx Jobs API
  slug: alteryx-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-jobs-api-openapi.yml
- filename: alteryx-schedules-api-openapi.yml
  format: yaml
  label: Alteryx Schedules API
  slug: alteryx-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-schedules-api-openapi.yml
- filename: alteryx-users-api-openapi.yml
  format: yaml
  label: Alteryx Users API
  slug: alteryx-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-users-api-openapi.yml
- filename: alteryx-workflows-api-openapi.yml
  format: yaml
  label: Alteryx Workflows API
  slug: alteryx-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/openapi/alteryx-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alteryx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trifacta.com
  spf: true
hosts:
- cert_expires: Oct 11 18:07:35 2026 GMT
  host: help.alteryx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 12:10:21 2026 GMT
  host: gallery.alteryx.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: api.trifacta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alteryx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alteryx, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alteryx
provider_slug: alteryx
slug: alteryx-domain-security
source_filename: alteryx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.alteryx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 18:07:35 2026 GMT\n  hsts: false\n- host: gallery.alteryx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 12:10:21 2026 GMT\n  hsts: null\n- host: api.trifacta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: alteryx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: trifacta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/security/alteryx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
---
