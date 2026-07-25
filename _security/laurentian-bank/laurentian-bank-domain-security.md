---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: laurentianbank.ca
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: www.laurentianbank.ca
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Laurentian Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laurentian Bank of Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Laurentian Bank of Canada
provider_slug: laurentian-bank
slug: laurentian-bank-domain-security
source_filename: laurentian-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laurentianbank.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: laurentianbank.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laurentian-bank/refs/heads/main/security/laurentian-bank-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Retail Banking
- Quebec
- Interac
- Data Aggregation
---
