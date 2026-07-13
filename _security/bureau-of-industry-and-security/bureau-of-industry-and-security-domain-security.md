---
api_specs:
- filename: bureau-of-industry-and-security-openapi.yml
  format: yaml
  label: Consolidated Screening List (CSL) API
  slug: consolidated-screening-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/openapi/bureau-of-industry-and-security-openapi.yml
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
- cert_expires: Sep  2 13:13:43 2026 GMT
  host: www.bis.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 10:56:42 2026 GMT
  host: www.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 10:56:42 2026 GMT
  host: api.trade.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bureau Of Industry And Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Industry and Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Industry and Security
provider_slug: bureau-of-industry-and-security
slug: bureau-of-industry-and-security-domain-security
source_filename: bureau-of-industry-and-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bis.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:13:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 10:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trade.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 10:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bis.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trade.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-industry-and-security/refs/heads/main/security/bureau-of-industry-and-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- Export Controls
- Federal Government
- Industries
- National Security
- Screening Lists
- Security
---
