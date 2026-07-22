---
description: ''
domains:
- caa: null
  dmarc: null
  dmarc_policy: null
  dnssec: null
  domain: letote.com
  note: Not "absent" — unmeasurable. The zone does not answer, so no record class can be evaluated either way.
  spf: null
hosts:
- error: SERVFAIL / could not resolve host
  host: letote.com
  hsts: null
  https: false
  resolves: false
  tls_version: null
- error: NXDOMAIN / could not resolve host
  host: www.letote.com
  hsts: null
  https: false
  resolves: false
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Le Tote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LE TOTE, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LE TOTE
provider_slug: le-tote
slug: le-tote-domain-security
source_filename: le-tote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig / whois / curl against letote.com on 2026-07-19\nsummary: >-\n  letote.com is still registered but is wholly unresolvable. The domain delegates\n  to four Amazon Route 53 nameservers that REFUSE the zone, meaning the hosted\n  zone was deleted while the NS records remained at the registrar — a dangling\n  delegation. Every DNS lookup returns SERVFAIL, so there is no A record, no\n  mail, no TLS endpoint, and no /.well-known surface to probe. This is consistent\n  with the company being defunct (see lifecycle/le-tote-lifecycle.yml).\nregistration:\n  domain: letote.com\n  registered: true\n  registrar: IONOS SE\n  registrar_iana_id: 83\n  creation_date: '2012-03-29'\n  updated_date: '2026-03-30'\n  status: ACTIVE\ndelegation:\n  resolves: false\n  resolution_status: SERVFAIL\n  dangling: true\n  registry_ns:\n  - ns-438.awsdns-54.com\n  - ns-614.awsdns-12.net\n  - ns-1197.awsdns-21.org\n  - ns-1867.awsdns-41.co.uk\n  authoritative_response:\
  \ REFUSED\n  note: >-\n    Route 53 nameservers answer REFUSED for letote.com, indicating no hosted zone\n    exists for the delegated domain. A dangling NS delegation of this shape is a\n    recognized domain-takeover risk vector should the zone name be re-claimed in\n    the same Route 53 namespace.\nhosts:\n- host: letote.com\n  resolves: false\n  https: false\n  tls_version: null\n  hsts: null\n  error: SERVFAIL / could not resolve host\n- host: www.letote.com\n  resolves: false\n  https: false\n  tls_version: null\n  hsts: null\n  error: NXDOMAIN / could not resolve host\ndomains:\n- domain: letote.com\n  dnssec: null\n  caa: null\n  spf: null\n  dmarc: null\n  dmarc_policy: null\n  note: >-\n    Not \"absent\" — unmeasurable. The zone does not answer, so no record class can\n    be evaluated either way.\nwell_known:\n  probed: false\n  reason: no resolvable host to probe /.well-known/ against\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/le-tote/refs/heads/main/security/le-tote-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Defunct
- Retail
- Fashion
- E-Commerce
- Clothing Rental
- Subscription Commerce
- Open Source
- Y Combinator
---
