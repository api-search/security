---
description: ''
domains:
- a_records: []
  aaaa_records: []
  caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: divshot.com
  mx: []
  nameservers:
  - a.share-dns.com.
  - b.share-dns.net.
  parked: true
  soa: null
  spf: false
- a_records:
  - 145.14.152.116
  caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: divshot.io
  nameservers:
  - orbit.dns-parking.com.
  - horizon.dns-parking.com.
  operated_by_provider: false
  spf: true
  spf_record: v=spf1 include:_spf.mail.hostinger.com ~all
hosts:
- error: could not connect (curl exit 6, could not resolve host)
  host: divshot.com
  http_status: null
  https: false
  resolves: false
- host: www.divshot.com
  resolves: false
- host: api.divshot.com
  resolves: false
- host: docs.divshot.com
  resolves: false
- detail: third-party WordPress 6.9.5 placeholder on Hostinger parking nameservers
  host: divshot.io
  http_status: 200
  https: true
  ip: 145.14.152.116
  operated_by_provider: false
  resolves: true
kind: domain-security
layout: security
method: probed
name: Divshot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divshot, probed live across 5 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Divshot
provider_slug: divshot
slug: divshot-domain-security
source_filename: divshot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: dig + curl probes run 2026-07-20\nnotes: >-\n  0-working/probe-domain-security.py reported `divshot unreachable` - the primary\n  domain does not resolve. The values below were probed directly. Absence of\n  records is real recorded data, not a gap in the probe. divshot.io, the old\n  app-hosting domain, now resolves to a third-party WordPress placeholder on\n  Hostinger and is NOT operated by Divshot - it is listed only so a later run\n  does not mistake it for a live Divshot surface.\nhosts:\n- host: divshot.com\n  resolves: false\n  https: false\n  http_status: null\n  error: could not connect (curl exit 6, could not resolve host)\n- host: www.divshot.com\n  resolves: false\n- host: api.divshot.com\n  resolves: false\n- host: docs.divshot.com\n  resolves: false\n- host: divshot.io\n  resolves: true\n  ip: 145.14.152.116\n  https: true\n  http_status: 200\n  operated_by_provider: false\n  detail: third-party WordPress 6.9.5\
  \ placeholder on Hostinger parking nameservers\ndomains:\n- domain: divshot.com\n  a_records: []\n  aaaa_records: []\n  mx: []\n  nameservers:\n  - a.share-dns.com.\n  - b.share-dns.net.\n  parked: true\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  soa: null\n- domain: divshot.io\n  operated_by_provider: false\n  a_records:\n  - 145.14.152.116\n  nameservers:\n  - orbit.dns-parking.com.\n  - horizon.dns-parking.com.\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.mail.hostinger.com ~all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divshot/refs/heads/main/security/divshot-domain-security.yml
summary_line: DMARC
tags:
- Company
- Web Hosting
- Static Hosting
- Front-End
- Deployment
- Developer Tools
- Defunct
- Acquired
---
