---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linkablenetworks.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: collinsongroup.com
  spf: true
hosts:
- cert_expires: Sep 29 17:24:43 2026 GMT
  host: linkablenetworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.collinsongroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:51:06 2026 GMT
  host: api.mylinkables.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkable Networks Collinson Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linkable Networks (Collinson Group), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Linkable Networks (Collinson Group)
provider_slug: linkable-networks-collinson-group
slug: linkable-networks-collinson-group-domain-security
source_filename: linkable-networks-collinson-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linkablenetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:24:43 2026 GMT\n  hsts: false\n- host: www.collinsongroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mylinkables.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:51:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linkablenetworks.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: collinsongroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkable-networks-collinson-group/refs/heads/main/security/linkable-networks-collinson-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Card Linked Offers
- Loyalty
- Payments
- Rewards
- Advertising
- Retail
---
