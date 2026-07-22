---
description: ''
domains:
- caa: []
  created: '2005-03-23'
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cerexa.com
  expires: '2027-03-23'
  mx: true
  mx_hosts:
  - mx1.hc3464-92.iphmx.com
  - mx2.hc3464-92.iphmx.com
  nameservers:
  - ns1.abbviedns.com
  - ns2.abbviedns.com
  - ns3.abbviedns.com
  - ns4.abbviedns.com
  registrant_operator: AbbVie
  registrar: MarkMonitor Inc.
  spf: true
  spf_record: v=spf1 include:_u.cerexa.com._spf.smart.ondmarc.com -all
hosts:
- a_record: 204.74.99.105
  host: cerexa.com
  hsts: false
  http: true
  http_status: 301
  https: false
  https_error: connection refused on port 443
  redirects_to: https://www.abbvie.com/allergan.html
- a_record: 204.74.99.105
  host: www.cerexa.com
  https: false
  https_error: connection refused on port 443
kind: domain-security
layout: security
method: probed
name: Cerexa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerexa, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cerexa
provider_slug: cerexa
slug: cerexa-domain-security
source_filename: cerexa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probe of cerexa.com (2026-07-20)\nnotes: >-\n  Cerexa is a defunct independent company. Its historical domain cerexa.com is\n  now registered and operated by AbbVie (MarkMonitor registrar, ns*.abbviedns.com\n  nameservers) and 301-redirects to https://www.abbvie.com/allergan.html. The\n  posture recorded below is therefore AbbVie's custodial posture over a legacy\n  domain, not a Cerexa-operated developer property.\nhosts:\n  - host: cerexa.com\n    https: false\n    https_error: connection refused on port 443\n    http: true\n    http_status: 301\n    redirects_to: https://www.abbvie.com/allergan.html\n    hsts: false\n    a_record: 204.74.99.105\n  - host: www.cerexa.com\n    https: false\n    https_error: connection refused on port 443\n    a_record: 204.74.99.105\ndomains:\n  - domain: cerexa.com\n    registrar: MarkMonitor Inc.\n    created: '2005-03-23'\n    expires: '2027-03-23'\n    nameservers:\n      - ns1.abbviedns.com\n\
  \      - ns2.abbviedns.com\n      - ns3.abbviedns.com\n      - ns4.abbviedns.com\n    registrant_operator: AbbVie\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: v=spf1 include:_u.cerexa.com._spf.smart.ondmarc.com -all\n    dmarc: true\n    dmarc_policy: none\n    mx: true\n    mx_hosts:\n      - mx1.hc3464-92.iphmx.com\n      - mx2.hc3464-92.iphmx.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerexa/refs/heads/main/security/cerexa-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Anti-Infectives
- Antibiotics
- Life Sciences
- Healthcare
- Acquired
---
