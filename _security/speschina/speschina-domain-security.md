---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: speschina.com
  mx:
  - mxn.mxhichina.com
  - mxw.mxhichina.com
  mx_provider: Alibaba Cloud (Aliyun / mxhichina)
  spf: false
hosts:
- a_record: 118.178.138.165
  cert_expires: '2027-03-08'
  cert_issuer: C=CN, O=Beijing Xinchacha Credit Management Co., Ltd., CN=Xcc Trust DV SSL CA
  host: www.speschina.com
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- host: speschina.com
  https: false
  note: apex resolves (121.43.159.115) but 443 connection times out; only the www host serves
kind: domain-security
layout: security
method: probed
name: Speschina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPES (speschina), probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SPES (speschina)
provider_slug: speschina
slug: speschina-domain-security
source_filename: speschina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + openssl s_client + curl HEAD (apex https://speschina.com times out on 443; www host serves)\nhosts:\n- host: www.speschina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: 'C=CN, O=Beijing Xinchacha Credit Management Co., Ltd., CN=Xcc Trust DV SSL CA'\n  cert_expires: '2027-03-08'\n  hsts: false\n  hsts_max_age: null\n  a_record: 118.178.138.165\n- host: speschina.com\n  https: false\n  note: apex resolves (121.43.159.115) but 443 connection times out; only the www host serves\ndomains:\n- domain: speschina.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx:\n  - mxn.mxhichina.com\n  - mxw.mxhichina.com\n  mx_provider: Alibaba Cloud (Aliyun / mxhichina)\nnotes: >-\n  Consumer brand marketing site (Vue/ElementUI SPA) hosted on Alibaba Cloud in China; no\n  public API surface. No HSTS, no CAA, no DNSSEC, and no SPF/DMARC email-authentication\n  records were published at probe\
  \ time. Absence of these records is recorded data, not an error.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speschina/refs/heads/main/security/speschina-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer Brand
- Personal Care
- Beauty
- E-commerce
- Direct to Consumer
- China
- No Public API
---
