---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: prosperitybankusa.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.prosperitybankusa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prosperity Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prosperity Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Prosperity Bank
provider_slug: prosperity-bank
slug: prosperity-bank-domain-security
source_filename: prosperity-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prosperitybankusa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: prosperitybankusa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosperity-bank/refs/heads/main/security/prosperity-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Regional Bank
- Texas
- Open Finance
- Data Aggregation
---
