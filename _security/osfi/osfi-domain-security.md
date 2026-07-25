---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gc.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bank-banque-canada.ca
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: www.osfi-bsif.gc.ca
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: connect-connexion.bank-banque-canada.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: open.canada.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osfi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSFI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OSFI
provider_slug: osfi
slug: osfi-domain-security
source_filename: osfi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osfi-bsif.gc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: connect-connexion.bank-banque-canada.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n- host: open.canada.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bank-banque-canada.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osfi/refs/heads/main/security/osfi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Regulator
- Life Insurance
- Property and Casualty
- Financial Regulation
- Prudential Supervision
- Open Data
- Risk Data
- Market Infrastructure
- Banking
- Basel III
- Capital Adequacy
- Regulatory Reporting
- Pensions
---
