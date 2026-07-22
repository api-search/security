---
description: ''
domains:
- caa: []
  creation_date: '2002-03-26'
  dmarc: false
  dnssec: false
  domain: yacob.com
  expiry_date: '2027-03-26'
  nameservers:
  - ns-cloud-a1.googledomains.com
  - ns-cloud-a2.googledomains.com
  - ns-cloud-a3.googledomains.com
  - ns-cloud-a4.googledomains.com
  registered: true
  registrar: GoDaddy.com, LLC
  spf: false
  zone_resolves: false
hosts:
- dns_status: SERVFAIL
  host: yacob.com
  https: false
  reachable: false
kind: domain-security
layout: security
method: probed
name: Yacob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yacob, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Yacob
provider_slug: yacob
slug: yacob-domain-security
source_filename: yacob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + whois + HTTPS probe (probe-domain-security.py reported host unreachable; manual dig/whois detail recorded)\nnote: >-\n  yacob.com is registered (GoDaddy, created 2002-03-26, expires 2027-03-26)\n  and delegated to Google Cloud DNS nameservers (ns-cloud-a1..a4.googledomains.com),\n  but those nameservers do not answer for the zone (SERVFAIL) — the DNS zone\n  appears deleted. No A, NS, MX, TXT, CAA, DS, or DMARC records resolve, and the\n  website is unreachable. The last non-parked archived copy of the site is from\n  2021 (web.archive.org); by March 2025 the domain served a GoDaddy parked lander.\nhosts:\n  - host: yacob.com\n    reachable: false\n    https: false\n    dns_status: SERVFAIL\ndomains:\n  - domain: yacob.com\n    registrar: GoDaddy.com, LLC\n    registered: true\n    creation_date: '2002-03-26'\n    expiry_date: '2027-03-26'\n    nameservers:\n      - ns-cloud-a1.googledomains.com\n      - ns-cloud-a2.googledomains.com\n\
  \      - ns-cloud-a3.googledomains.com\n      - ns-cloud-a4.googledomains.com\n    zone_resolves: false\n    dnssec: false\n    caa: []\n    spf: false\n    dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yacob/refs/heads/main/security/yacob-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Nutrition
- Education
- Payments
- Cashless Payments
- Schools
- Parenting
- United Arab Emirates
---
