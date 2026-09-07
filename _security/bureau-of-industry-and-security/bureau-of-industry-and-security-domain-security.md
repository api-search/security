---
api_specs:
- filename: bureau-of-industry-and-security-csl-apim-export.yaml
  format: yaml
  label: Consolidated Screening List (CSL) API
  slug: consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/_original/bureau-of-industry-and-security-csl-apim-export.yaml
- filename: bureau-of-industry-and-security-search-api-openapi.yml
  format: yaml
  label: Bureau of Industry and Security Search API
  slug: bureau-of-industry-and-security-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/bureau-of-industry-and-security-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bis.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trade.gov
  spf: true
hosts:
- cert_expires: Oct 31 13:28:45 2026 GMT
  host: www.bis.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.trade.gov
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Bureau Of Industry And Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Industry and Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Industry and Security
provider_slug: bureau-of-industry-and-security
slug: bureau-of-industry-and-security-domain-security
source_filename: bureau-of-industry-and-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bis.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trade.gov\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: bis.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trade.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/security/bureau-of-industry-and-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Export Controls
- Federal-Government
- Industries
- National Security
- Screening Lists
- Security
---
