---
description: ''
domains:
- a_record: false
  aaaa_record: false
  caa: []
  dmarc: false
  dnssec: false
  domain: tugboatyards.com
  mx:
  - mx.hover.com.cust.hostedemail.com
  nameservers:
  - ns1.hover.com
  - ns2.hover.com
  registered: true
  spf: false
  txt: []
hosts:
- error: DNS does not resolve (no A/AAAA record; curl "Could not resolve host")
  host: tugboatyards.com
  https: false
  reachable: false
- error: DNS does not resolve (curl "Could not resolve host")
  host: www.tugboatyards.com
  https: false
  reachable: false
- error: parent zone has no A/AAAA records; historical API host (archived 302 capture 2015-05-24 redirecting to tugboatyards.com/developer/api)
  host: api.tugboatyards.com
  https: false
  reachable: false
kind: domain-security
layout: security
method: probed
name: Tugboat Yards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tugboat Yards, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tugboat Yards
provider_slug: tugboat-yards
slug: tugboat-yards-domain-security
source_filename: tugboat-yards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nnote: Tugboat Yards is defunct. The tugboatyards.com domain is still registered\n  (Hover nameservers and MX remain) but publishes no A/AAAA records, so neither\n  the website nor the former api.tugboatyards.com host is reachable. Absence of\n  records below is observed data, probed 2026-07-21 with dig and curl.\nhosts:\n- host: tugboatyards.com\n  https: false\n  reachable: false\n  error: DNS does not resolve (no A/AAAA record; curl \"Could not resolve host\")\n- host: www.tugboatyards.com\n  https: false\n  reachable: false\n  error: DNS does not resolve (curl \"Could not resolve host\")\n- host: api.tugboatyards.com\n  https: false\n  reachable: false\n  error: parent zone has no A/AAAA records; historical API host (archived 302\n    capture 2015-05-24 redirecting to tugboatyards.com/developer/api)\ndomains:\n- domain: tugboatyards.com\n  registered: true\n  nameservers: [ns1.hover.com, ns2.hover.com]\n  a_record: false\n  aaaa_record:\
  \ false\n  mx: [mx.hover.com.cust.hostedemail.com]\n  dnssec: false\n  caa: []\n  spf: false\n  txt: []\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tugboat-yards/refs/heads/main/security/tugboat-yards-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Media
- Publishing
- Crowdfunding
- Audience Funding
- Payments
- Defunct
---
