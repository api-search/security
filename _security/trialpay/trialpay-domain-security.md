---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: trialpay.com
  nameservers:
  - awsdns-24.net
  - awsdns-35.org
  - awsdns-06.co.uk
  - awsdns-51.com
  spf: true
  spf_record: v=spf1 a mx ip4:54.183.233.157 ip4:54.183.231.95 ip4:52.8.133.87 ip4:50.18.203.174 include:aspmx.googlemail.com include:amazonses.com ~all
hosts:
- host: www.trialpay.com
  https: false
  note: DNS resolves (AWS) but HTTPS connection times out
  reachable: false
- host: trialpay.com
  https: false
  note: DNS resolves (AWS) but HTTPS connection times out
  reachable: false
  resolves_to:
  - 52.9.34.236
  - 54.177.189.139
- host: help.trialpay.com
  https: false
  note: NXDOMAIN — former developer docs host no longer resolves
  reachable: false
kind: domain-security
layout: security
method: probed
name: Trialpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrialPay, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TrialPay
provider_slug: trialpay
slug: trialpay-domain-security
source_filename: trialpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + HTTPS HEAD against trialpay.com (2026-07-21)\nnote: >-\n  TrialPay was acquired by Visa in April 2015 and folded into the Visa Commerce\n  Network. The trialpay.com domain is still registered (AWS Route 53 nameservers,\n  Amazon SES / Google Workspace mail per SPF) but the public web/API servers no\n  longer respond over HTTPS, and the former developer docs host help.trialpay.com\n  no longer resolves. Absence of records below is real, recorded data.\nhosts:\n  - host: www.trialpay.com\n    https: false\n    reachable: false\n    note: DNS resolves (AWS) but HTTPS connection times out\n  - host: trialpay.com\n    https: false\n    reachable: false\n    resolves_to: [52.9.34.236, 54.177.189.139]\n    note: DNS resolves (AWS) but HTTPS connection times out\n  - host: help.trialpay.com\n    https: false\n    reachable: false\n    note: NXDOMAIN — former developer docs host no longer resolves\ndomains:\n  - domain: trialpay.com\n\
  \    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 a mx ip4:54.183.233.157 ip4:54.183.231.95 ip4:52.8.133.87 ip4:50.18.203.174 include:aspmx.googlemail.com include:amazonses.com ~all\"\n    dmarc: false\n    dmarc_policy: null\n    nameservers: [awsdns-24.net, awsdns-35.org, awsdns-06.co.uk, awsdns-51.com]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trialpay/refs/heads/main/security/trialpay-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Payments
- Advertising
- Monetization
- Offer Wall
- Gaming
- Mobile
- Acquired
---
