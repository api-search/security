---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equitablebank.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eqbank.ca
  spf: true
hosts:
- cert_expires: Oct 14 21:04:33 2026 GMT
  host: www.equitablebank.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 21:02:32 2026 GMT
  host: www.eqbank.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 15:40:33 2026 GMT
  host: eqb.investorroom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Equitable Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equitable Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equitable Bank
provider_slug: equitable-bank
slug: equitable-bank-domain-security
source_filename: equitable-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equitablebank.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:04:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eqbank.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 21:02:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: eqb.investorroom.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 18 15:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: equitablebank.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eqbank.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equitable-bank/refs/heads/main/security/equitable-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Schedule I Bank
- Digital Banking
- Open Banking
- Consumer-Driven Banking
- Data Aggregation
- Challenger Bank
---
