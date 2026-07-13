---
api_specs:
- filename: splunk-enterprise-rest-api.yml
  format: yaml
  label: Splunk Enterprise REST API
  slug: splunk-enterprise-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/openapi/splunk-enterprise-rest-api.yml
- filename: openapi.json
  format: json
  label: Splunk Cloud ACS OpenAPI Specification
  slug: splunk-cloud-admin-config-service-openapi
  spec_type: OpenAPI
  url: https://admin.splunk.com/service/info/specs/v2/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: splunk.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.splunk.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: docs.splunk.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 29 00:41:29 2026 GMT
  host: help.splunk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Splunk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Splunk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Splunk
provider_slug: splunk
slug: splunk-domain-security
source_filename: splunk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.splunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: docs.splunk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: null\n- host: help.splunk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:41:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: splunk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/security/splunk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
---
