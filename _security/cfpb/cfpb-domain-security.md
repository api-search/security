---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Consumer Complaint Database API
  slug: consumer-complaint-database-api
  spec_type: OpenAPI
  url: https://cfpb.github.io/ccdb5-api/documentation/
- filename: cfpb-hmda-data-browser-api-openapi.yml
  format: yaml
  label: HMDA Data Browser API
  slug: hmda-data-browser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/main/openapi/cfpb-hmda-data-browser-api-openapi.yml
- filename: cfpb-hmda-filing-api-openapi.yml
  format: yaml
  label: HMDA Platform Filing API
  slug: hmda-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/main/openapi/cfpb-hmda-filing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: consumerfinance.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfpb.gov
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: www.consumerfinance.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: ffiec.cfpb.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cfpb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Financial Protection Bureau (CFPB), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Financial Protection Bureau (CFPB)
provider_slug: cfpb
slug: cfpb-domain-security
source_filename: cfpb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.consumerfinance.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\n- host: ffiec.cfpb.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: consumerfinance.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cfpb.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/security/cfpb-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Consumer Finance
- Government
- Complaints
- Mortgage
- HMDA
- Financial Data
- Regulatory
- Open Data
---
