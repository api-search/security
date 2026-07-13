---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citizensbank.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.citizensbank.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: developer.citizensbank.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- host: developer-citizenspay.citizensbank.com
  https: false
kind: domain-security
layout: security
method: probed
name: Citizens Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citizens Financial Group, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citizens Financial Group
provider_slug: citizens-financial-group
slug: citizens-financial-group-domain-security
source_filename: citizens-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citizensbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.citizensbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer-citizenspay.citizensbank.com\n  https: false\ndomains:\n- domain: citizensbank.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citizens-financial-group/refs/heads/main/security/citizens-financial-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Buy Now Pay Later
- Financial Services
- FDX
- Locator
- Open Banking
- Payments
---
