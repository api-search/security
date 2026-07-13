---
api_specs:
- filename: index.htm
  format: yaml
  label: The Bureau of Economic Analysis API
  slug: the-bureau-of-economic-analysis
  spec_type: OpenAPI
  url: https://apps.bea.gov/API/docs/index.htm
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bea.gov
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.bea.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: apps.bea.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Bureau Of Economic Analysis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Bureau of Economic Analysis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Bureau of Economic Analysis
provider_slug: the-bureau-of-economic-analysis
slug: the-bureau-of-economic-analysis-domain-security
source_filename: the-bureau-of-economic-analysis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bea.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apps.bea.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bea.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-bureau-of-economic-analysis/refs/heads/main/security/the-bureau-of-economic-analysis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Economics
- Federal Government
- GDP
- National Accounts
- Open Data
- Statistics
---
