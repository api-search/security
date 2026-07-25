---
api_specs:
- filename: bloomberg-apis-apiauth-api-openapi.yml
  format: yaml
  label: Bloomberg APIs apiauth API
  slug: bloomberg-apis-apiauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-apiauth-api-openapi.yml
- filename: bloomberg-apis-apiflds-api-openapi.yml
  format: yaml
  label: Bloomberg APIs apiflds API
  slug: bloomberg-apis-apiflds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-apiflds-api-openapi.yml
- filename: bloomberg-apis-instruments-api-openapi.yml
  format: yaml
  label: Bloomberg APIs instruments API
  slug: bloomberg-apis-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-instruments-api-openapi.yml
- filename: bloomberg-apis-mktbar-api-openapi.yml
  format: yaml
  label: Bloomberg APIs mktbar API
  slug: bloomberg-apis-mktbar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktbar-api-openapi.yml
- filename: bloomberg-apis-mktdata-api-openapi.yml
  format: yaml
  label: Bloomberg APIs mktdata API
  slug: bloomberg-apis-mktdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktdata-api-openapi.yml
- filename: bloomberg-apis-mktvwap-api-openapi.yml
  format: yaml
  label: Bloomberg APIs mktvwap API
  slug: bloomberg-apis-mktvwap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-mktvwap-api-openapi.yml
- filename: bloomberg-apis-pagedata-api-openapi.yml
  format: yaml
  label: Bloomberg APIs pagedata API
  slug: bloomberg-apis-pagedata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-pagedata-api-openapi.yml
- filename: bloomberg-apis-refdata-api-openapi.yml
  format: yaml
  label: Bloomberg APIs refdata API
  slug: bloomberg-apis-refdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-refdata-api-openapi.yml
- filename: bloomberg-apis-tasvc-api-openapi.yml
  format: yaml
  label: Bloomberg APIs tasvc API
  slug: bloomberg-apis-tasvc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/openapi/bloomberg-apis-tasvc-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:reportvuln@bloomberg.net"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bloomberg.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: developer.bloomberg.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.bloomberg.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bloomberg Apis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg APIs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg APIs
provider_slug: bloomberg-apis
slug: bloomberg-apis-domain-security
source_filename: bloomberg-apis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-apis/refs/heads/main/security/bloomberg-apis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Financial Data
- Market Data
- News
- Terminal
---
