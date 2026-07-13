---
api_specs:
- filename: salesforce-net-zero-cloud-rest-api-openapi.yml
  format: yaml
  label: Net Zero Cloud REST API
  slug: net-zero-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/openapi/salesforce-net-zero-cloud-rest-api-openapi.yml
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
- host: yourinstance.my.salesforce.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Net Zero Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Net Zero Cloud, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Net Zero Cloud
provider_slug: salesforce-net-zero-cloud
slug: salesforce-net-zero-cloud-domain-security
source_filename: salesforce-net-zero-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: yourinstance.my.salesforce.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/security/salesforce-net-zero-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Environmental
- ESG
- Net Zero
- Sustainability
---
