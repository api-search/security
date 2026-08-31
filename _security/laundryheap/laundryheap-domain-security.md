---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laundryheap.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.laundryheap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laundryheap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laundryheap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laundryheap
provider_slug: laundryheap
slug: laundryheap-domain-security
source_filename: laundryheap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laundryheap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: laundryheap.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laundryheap/refs/heads/main/security/laundryheap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Laundry
- Dry Cleaning
- On-Demand Services
- Logistics
- Last Mile Delivery
- Consumer Services
- Hospitality
- Ordering
- GraphQL
- Authentication
---
