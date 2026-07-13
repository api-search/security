---
api_specs:
- filename: blpapi-core.yml
  format: yaml
  label: Bloomberg BLPAPI Core
  slug: bloomberg-blpapi-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/openapi/blpapi-core.yml
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
name: Bloomberg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bloomberg, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bloomberg
provider_slug: bloomberg
slug: bloomberg-domain-security
source_filename: bloomberg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bloomberg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bloomberg.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:reportvuln@bloomberg.net\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bloomberg/refs/heads/main/security/bloomberg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Data License
- Enterprise
- Execution Management
- Financial Services
- Market Data
- News
- Quantitative Analysis
- Trading
- Transaction Cost Analysis
---
