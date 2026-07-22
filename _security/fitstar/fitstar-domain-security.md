---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; P=none; rua=mailto:dmarc-reports@fitstar.com
  dnssec: false
  domain: fitstar.com
  mx: true
  mx_records:
  - 5 alt1.aspmx.l.google.com.
  - 5 alt2.aspmx.l.google.com.
  - 10 alt3.aspmx.l.google.com.
  - 10 alt4.aspmx.l.google.com.
  nameservers:
  - ns-cloud-b1.googledomains.com.
  - ns-cloud-b2.googledomains.com.
  - ns-cloud-b3.googledomains.com.
  - ns-cloud-b4.googledomains.com.
  spf: true
  spf_record: v=spf1 ip4:13.111.15.117 ip4:13.111.15.118 include:_spf.google.com include:_spf.salesforce.com ~all
hosts:
- a_records: []
  host: fitstar.com
  hsts: null
  https: false
  note: NS delegated but no A record; host does not resolve
  resolves: false
  tls_version: null
- a_records: []
  host: www.fitstar.com
  https: false
  note: does not resolve
  resolves: false
- a_records: []
  host: api.fitstar.com
  https: false
  note: does not resolve
  resolves: false
- a_records: []
  host: developer.fitstar.com
  https: false
  note: does not resolve
  resolves: false
kind: domain-security
layout: security
method: probed
name: Fitstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FitStar, probed live across 4 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FitStar
provider_slug: fitstar
slug: fitstar-domain-security
source_filename: fitstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig probe of fitstar.com (2026-07-20)\nnote: >-\n  FitStar Labs, Inc. is defunct — acquired by Fitbit on 2015-03-05 and wound down.\n  The fitstar.com domain is still registered and actively administered (Google Cloud\n  DNS, Google Workspace mail, Salesforce SPF include, CAA restricted to pki.goog),\n  but it publishes NO A record and serves no web content, so there are no HTTPS/TLS\n  or HSTS observations to record. Mail and DNS posture is recorded because it is real\n  probed data; absence of web hosts is a valid, expected result.\nhosts:\n  - host: fitstar.com\n    a_records: []\n    https: false\n    resolves: false\n    tls_version: null\n    hsts: null\n    note: NS delegated but no A record; host does not resolve\n  - host: www.fitstar.com\n    a_records: []\n    https: false\n    resolves: false\n    note: does not resolve\n  - host: api.fitstar.com\n    a_records: []\n    https: false\n    resolves: false\n    note:\
  \ does not resolve\n  - host: developer.fitstar.com\n    a_records: []\n    https: false\n    resolves: false\n    note: does not resolve\ndomains:\n  - domain: fitstar.com\n    nameservers:\n      - ns-cloud-b1.googledomains.com.\n      - ns-cloud-b2.googledomains.com.\n      - ns-cloud-b3.googledomains.com.\n      - ns-cloud-b4.googledomains.com.\n    dnssec: false\n    caa:\n      - 0 issue \"pki.goog\"\n    spf: true\n    spf_record: 'v=spf1 ip4:13.111.15.117 ip4:13.111.15.118 include:_spf.google.com include:_spf.salesforce.com ~all'\n    dmarc: true\n    dmarc_policy: none\n    dmarc_record: 'v=DMARC1; P=none; rua=mailto:dmarc-reports@fitstar.com'\n    mx: true\n    mx_records:\n      - 5 alt1.aspmx.l.google.com.\n      - 5 alt2.aspmx.l.google.com.\n      - 10 alt3.aspmx.l.google.com.\n      - 10 alt4.aspmx.l.google.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fitstar/refs/heads/main/security/fitstar-domain-security.yml
summary_line: DMARC
tags:
- Company
- Defunct
- Acquired
- Fitness
- Health and Wellness
- Consumer Applications
- Mobile Applications
- Personal Training
---
