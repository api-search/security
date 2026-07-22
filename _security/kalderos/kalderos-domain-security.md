---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kalderos.com
  spf: true
hosts:
- cert_expires: Oct  1 16:56:35 2026 GMT
  host: www.kalderos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kalderos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kalderos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kalderos
provider_slug: kalderos
slug: kalderos-domain-security
source_filename: kalderos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kalderos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 16:56:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kalderos.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kalderos/refs/heads/main/security/kalderos-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Healthcare
- 340B
- Drug Discounts
- Rebate Management
- Compliance
- Life Sciences
- Pharmaceutical
- Medicaid
- Health Tech
---
