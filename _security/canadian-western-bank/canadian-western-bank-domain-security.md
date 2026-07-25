---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cwbank.com
  spf: true
hosts:
- cert_expires: Jan  2 15:44:38 2027 GMT
  host: www.cwbank.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canadian Western Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canadian Western Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canadian Western Bank
provider_slug: canadian-western-bank
slug: canadian-western-bank-domain-security
source_filename: canadian-western-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cwbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 15:44:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: cwbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canadian-western-bank/refs/heads/main/security/canadian-western-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Business Banking
- Alberta
- Open Finance
- Consumer-Driven Banking
- Data Aggregation
---
