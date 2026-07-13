---
api_specs:
- filename: openapi.json
  format: json
  label: Service Cloud REST API
  slug: service-cloud-rest-api
  spec_type: OpenAPI
  url: https://api.salesforce.com/service-cloud/openapi.json
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
kind: domain-security
layout: security
method: probed
name: Service Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Service Cloud APIs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Service Cloud APIs
provider_slug: service-cloud
slug: service-cloud-domain-security
source_filename: service-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/security/service-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud
- CRM
- Customer-Service
- Enterprise
- Salesforce
- Support
---
