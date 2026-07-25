---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fnbc.ca
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.fnbc.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Nations Bank Of Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Nations Bank of Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: First Nations Bank of Canada
provider_slug: first-nations-bank-of-canada
slug: first-nations-bank-of-canada-domain-security
source_filename: first-nations-bank-of-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fnbc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fnbc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-nations-bank-of-canada/refs/heads/main/security/first-nations-bank-of-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Indigenous
- Consumer-Driven Banking
- Data Aggregation
- Interac
---
