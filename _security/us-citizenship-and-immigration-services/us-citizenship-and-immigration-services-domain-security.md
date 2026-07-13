---
api_specs:
- filename: uscis-case-status-api-openapi.yml
  format: yaml
  label: USCIS Case Status API
  slug: uscis-case-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-case-status-api-openapi.yml
- filename: uscis-foia-api-openapi.yml
  format: yaml
  label: USCIS FOIA Request and Status API
  slug: uscis-foia-request-and-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/openapi/uscis-foia-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: uscis.gov
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: developer.uscis.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api-int.uscis.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Citizenship And Immigration Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Citizenship and Immigration Services, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Citizenship and Immigration Services
provider_slug: us-citizenship-and-immigration-services
slug: us-citizenship-and-immigration-services-domain-security
source_filename: us-citizenship-and-immigration-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.uscis.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-int.uscis.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: uscis.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-citizenship-and-immigration-services/refs/heads/main/security/us-citizenship-and-immigration-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Immigration
- Citizenship
- Case Status
- FOIA
---
