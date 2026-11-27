---
api_specs:
- filename: wfhalert-com-health-api-openapi.yml
  format: yaml
  label: WFH Alert Health API
  slug: wfhalert-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wfhalert-com/openapi/wfhalert-com-health-api-openapi.yml
- filename: wfhalert-com-integrations-api-openapi.yml
  format: yaml
  label: WFH Alert Integrations API
  slug: wfhalert-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wfhalert-com/openapi/wfhalert-com-integrations-api-openapi.yml
- filename: wfhalert-com-jobs-api-openapi.yml
  format: yaml
  label: WFH Alert Jobs API
  slug: wfhalert-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wfhalert-com/openapi/wfhalert-com-jobs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wfhalert.com
  spf: true
hosts:
- cert_expires: Jan 19 11:46:18 2027 GMT
  host: www.wfhalert.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WFH Alert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WFH Alert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WFH Alert
provider_slug: wfhalert-com
slug: wfhalert-com-domain-security
source_filename: wfhalert-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wfhalert.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 11:46:18 2027 GMT\n  hsts: false\ndomains:\n- domain: wfhalert.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wfhalert-com/security/wfhalert-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Remote Jobs
- Job Alerts
- Entry-Level
- Data Entry
- Customer Service
---
