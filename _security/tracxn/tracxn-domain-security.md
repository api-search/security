---
api_specs:
- filename: overview
  format: yaml
  label: Tracxn API
  slug: tracxn-api
  spec_type: Postman
  url: https://www.postman.com/tracxnapi/tracxn-api/overview
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: tracxn.com
  spf: true
hosts:
- cert_expires: Oct 11 04:32:02 2026 GMT
  host: tracxn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 03:48:45 2026 GMT
  host: w.tracxn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 04:32:02 2026 GMT
  host: platform.tracxn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tracxn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tracxn, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tracxn
provider_slug: tracxn
slug: tracxn-domain-security
source_filename: tracxn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tracxn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 04:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: w.tracxn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 03:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.tracxn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 04:32:02 2026 GMT\n  hsts: null\ndomains:\n- domain: tracxn.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tracxn/refs/heads/main/security/tracxn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cloud Saas
- Market Intelligence
- Private Markets
- Venture Capital
- Startups
- Company Data
- Investors
- Funding
---
