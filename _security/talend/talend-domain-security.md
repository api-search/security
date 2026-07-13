---
api_specs:
- filename: talend-orchestration-openapi.yml
  format: yaml
  label: Talend Cloud Orchestration API
  slug: talend-orchestration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-orchestration-openapi.yml
- filename: talend-processing-openapi.yml
  format: yaml
  label: Talend Cloud Processing API
  slug: talend-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/openapi/talend-processing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talend.com
  spf: true
hosts:
- cert_expires: Sep 24 02:53:47 2026 GMT
  host: talend.qlik.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 20:15:14 2026 GMT
  host: www.talend.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talend, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Talend
provider_slug: talend
slug: talend-domain-security
source_filename: talend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talend.qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.talend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:15:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: talend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talend/refs/heads/main/security/talend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Management
- Data Integration
- Data Quality
- ETL
- Orchestration
- Pipelines
---
