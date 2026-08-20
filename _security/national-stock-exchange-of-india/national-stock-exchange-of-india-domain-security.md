---
description: ''
domains:
- caa:
  - 2 issue "letsencrypt.org"
  - 1 issue "pki.goog"
  - 0 issue "www.digicert.com"
  - 3 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nseindia.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.nseindia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: bricsonline.nseindia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: eofs.nseindia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Stock Exchange Of India Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Stock Exchange of India, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Stock Exchange of India
provider_slug: national-stock-exchange-of-india
slug: national-stock-exchange-of-india-domain-security
source_filename: national-stock-exchange-of-india-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nseindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\n- host: bricsonline.nseindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\n- host: eofs.nseindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nseindia.com\n  dnssec: true\n  caa:\n  - 2 issue \"letsencrypt.org\"\n  - 1 issue \"pki.goog\"\n  - 0 issue \"www.digicert.com\"\n  - 3 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-stock-exchange-of-india/refs/heads/main/security/national-stock-exchange-of-india-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Stock Exchange
- Capital Markets
- Market Data
- Trading
- Financial-Services
- Securities
- India
- FIX Protocol
- Bonds
---
