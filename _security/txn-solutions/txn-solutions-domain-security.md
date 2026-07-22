---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: txn.com
  mx: false
  nameservers:
  - ns1.ename.net
  - ns2.ename.net
  spf: false
hosts:
- dns_a: 8.218.163.58
  host: txn.com
  hsts: false
  https: true
  tls_self_signed: true
- dns_a: 8.218.163.58
  host: www.txn.com
kind: domain-security
layout: security
method: probed
name: Txn Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TXN Solutions, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TXN Solutions
provider_slug: txn-solutions
slug: txn-solutions-domain-security
source_filename: txn-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS probe of txn.com (historical company domain)\nnote: >-\n  txn.com is the historical domain of TXN Solutions (TXN), a 2014-founded\n  transaction-data analytics startup that appears to be defunct. As of this\n  probe the domain no longer appears to be operated by the company: its\n  nameservers point to the eName domain marketplace (ns1/ns2.ename.net, SOA\n  admin.ename.net), the apex resolves to an Alibaba Cloud IP (8.218.163.58),\n  HTTPS terminates with a self-signed certificate (confirmed via two\n  independent fetch paths), and the zone publishes no MX, SPF, or DMARC\n  records. This record documents the historical association only; it is not\n  evidence about any live company infrastructure.\nhosts:\n  - host: txn.com\n    dns_a: 8.218.163.58\n    https: true\n    tls_self_signed: true\n    hsts: false\n  - host: www.txn.com\n    dns_a: 8.218.163.58\ndomains:\n  - domain: txn.com\n    nameservers:\n      - ns1.ename.net\n\
  \      - ns2.ename.net\n    dnssec: false\n    caa: []\n    mx: false\n    spf: false\n    dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/txn-solutions/refs/heads/main/security/txn-solutions-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Fintech
- Transaction Data
- Consumer Spending
- Market Research
- Analytics
---
