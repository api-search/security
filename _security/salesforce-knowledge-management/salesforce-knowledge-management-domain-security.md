---
api_specs:
- filename: salesforce-knowledge-management-rest-api-openapi.yml
  format: yaml
  label: Salesforce Knowledge REST API
  slug: salesforce-knowledge-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/openapi/salesforce-knowledge-management-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: yourinstance.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Knowledge Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Knowledge Management, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
slug: salesforce-knowledge-management-domain-security
source_filename: salesforce-knowledge-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: yourinstance.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/security/salesforce-knowledge-management-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
---
