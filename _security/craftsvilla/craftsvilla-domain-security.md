---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: craftsvilla.com
  mx: true
  mx_hosts:
  - aspmx.l.google.com
  - alt1.aspmx.l.google.com
  - alt2.aspmx.l.google.com
  - aspmx2.googlemail.com
  - aspmx3.googlemail.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:amazonses.com ~all
hosts:
- detail: HTTP 301 -> https://www.craftsvilla.com/ (AmazonS3); HTTPS root connection timed out; www is NXDOMAIN
  host: craftsvilla.com
  https: false
  reachable: false
kind: domain-security
layout: security
method: probed
name: Craftsvilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craftsvilla, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Craftsvilla
provider_slug: craftsvilla
slug: craftsvilla-domain-security
source_filename: craftsvilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: dig + TLS/HTTP probe of craftsvilla.com\nnotes: >-\n  Storefront is defunct. craftsvilla.com is served from an AWS S3 bucket that\n  301-redirects to https://www.craftsvilla.com/, but www.craftsvilla.com does not\n  resolve (NXDOMAIN) and the HTTPS root times out. No live website, API host, or\n  developer surface. The registrable domain still carries DNS records (probed\n  below); absence of a record is valid recorded data.\nhosts:\n  - host: craftsvilla.com\n    https: false\n    reachable: false\n    detail: HTTP 301 -> https://www.craftsvilla.com/ (AmazonS3); HTTPS root connection timed out; www is NXDOMAIN\ndomains:\n  - domain: craftsvilla.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:_spf.google.com include:spf.mandrillapp.com include:amazonses.com ~all\"\n    dmarc: false\n    dmarc_policy: null\n    mx: true\n    mx_hosts:\n      - aspmx.l.google.com\n      - alt1.aspmx.l.google.com\n\
  \      - alt2.aspmx.l.google.com\n      - aspmx2.googlemail.com\n      - aspmx3.googlemail.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craftsvilla/refs/heads/main/security/craftsvilla-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- E-Commerce
- Marketplace
- Retail
- Fashion
- Ethnic Wear
- Handcrafted
- India
---
