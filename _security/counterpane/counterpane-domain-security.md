---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: counterpane.com
  mx: []
  nameservers:
  - ns11.worldnic.com.
  - ns12.worldnic.com.
  spf: false
hosts:
- address: 209.17.116.163
  host: counterpane.com
  hsts: false
  http: true
  http_redirects_to: https://www.schneier.com/
  http_status: 301
  https: false
  https_error: connection refused on port 443
  resolves: true
- host: www.counterpane.com
  hsts: false
  http: true
  http_status: 404
  https: false
  https_error: connection refused on port 443
  resolves: true
kind: domain-security
layout: security
method: probed
name: Counterpane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Counterpane, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Counterpane
provider_slug: counterpane
slug: counterpane-domain-security
source_filename: counterpane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: 'live probe (dig + TLS connect + HTTP HEAD) of counterpane.com on 2026-07-20'\nnote: >-\n  Counterpane is defunct (acquired by BT Group in 2006). The domain is still registered and resolves,\n  but serves no site of its own: HTTPS on port 443 is refused, and plain HTTP 301-redirects every path\n  to https://www.schneier.com/ (Bruce Schneier's personal site). Absence of records below is real\n  observed data for a dormant domain, not a gap in the probe.\nhosts:\n- host: counterpane.com\n  resolves: true\n  address: 209.17.116.163\n  https: false\n  https_error: connection refused on port 443\n  http: true\n  http_status: 301\n  http_redirects_to: https://www.schneier.com/\n  hsts: false\n- host: www.counterpane.com\n  resolves: true\n  https: false\n  https_error: connection refused on port 443\n  http: true\n  http_status: 404\n  hsts: false\ndomains:\n- domain: counterpane.com\n  nameservers:\n  - ns11.worldnic.com.\n  - ns12.worldnic.com.\n\
  \  dnssec: false\n  caa: []\n  mx: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nwell_known:\n- path: /.well-known/security.txt\n  status: 301\n  note: blanket redirect to schneier.com; no document served\n- path: /.well-known/openid-configuration\n  status: 301\n  note: blanket redirect to schneier.com; no document served\n- path: /.well-known/api-catalog\n  status: 301\n  note: blanket redirect to schneier.com; no document served\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/counterpane/refs/heads/main/security/counterpane-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Cybersecurity
- Managed Security Services
- Security Monitoring
- Defunct
- Acquired
- Historical
---
