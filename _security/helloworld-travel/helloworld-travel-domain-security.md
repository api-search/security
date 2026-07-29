---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: helloworldlimited.com.au
  note: corporate domain publishes SPF with a soft fail and no DMARC record
  spf: true
  spf_record: v=spf1 include:zoho.com ~all
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_delegated: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: helloworld.com.au
  spf: true
  spf_record: v=spf1 include:_spf.helloworld_com_au._d.easydmarc.pro -all
- caa: []
  dmarc: true
  dmarc_delegated: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: readyrooms.com.au
  note: DMARC aggregate and forensic reporting is split between EasyDMARC and Proofpoint
  spf: true
  spf_record: v=spf1 include:_spf.readyrooms_com_au._d.easydmarc.pro ~all
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: false
  dnssec: false
  domain: aotonline.net
  note: the inbound trade booking domain publishes neither SPF nor DMARC
  spf: false
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_delegated: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: airtickets.com.au
  spf: true
  spf_record: v=spf1 include:_spf.airtickets_com_au._d.easydmarc.pro -all
- caa: []
  dmarc: true
  dmarc_delegated: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: expresstickets.com.au
  spf: true
  spf_record: v=spf1 include:_spf.expresstickets_com_au._d.easydmarc.pro -all
hosts:
- cert_expires: Sep 16 02:43:16 2026 GMT
  host: www.helloworldlimited.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  role: corporate website
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:43:16 2026 GMT
  host: policies.helloworldlimited.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  role: privacy and cookie policy host
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:32:30 2026 GMT
  host: www.helloworld.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 301
  https: true
  role: consumer website (redirects to /Find-Your-Agent.html)
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:04:20 2026 GMT
  host: www.readyrooms.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: covered by the wildcard certificate *.readyrooms.com.au
  role: ReadyRooms B2B hotel and activity booking, agent login
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:04:20 2026 GMT
  host: athena.readyrooms.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  role: ReadyRooms agent login application
  tls_version: TLSv1.3
- cert_expires: Oct  6 06:04:20 2026 GMT
  host: developer.readyrooms.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 401
  https: true
  note: 'HTTP Basic on every path (WWW-Authenticate: Basic realm="Access is permitted to authorized users"). HSTS is served on the 401 response itself.'
  role: provisioned but gated developer host
  tls_version: TLSv1.3
- cert_expires: Sep 14 01:14:40 2026 GMT
  host: www.aotonline.net
  hsts: true
  hsts_max_age: 31536000
  http_status: 302
  https: true
  role: AOTonline.net inbound trade booking engine, agency-code login
  tls_version: TLSv1.3
- cert_expires: Sep  7 01:12:43 2026 GMT
  host: www.airtickets.com.au
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: host returns HTTP 200 with an empty body for every unknown path (soft 404)
  role: Air Tickets / SmartTickets consolidation, agent login
  tls_version: TLSv1.3
- cert_expires: Oct  9 04:59:20 2026 GMT
  host: expresstickets.com.au
  hsts: false
  http_status: 403
  https: true
  note: Edge returns 403 to a scripted client on every path; no Strict-Transport-Security header was present on that response.
  role: Express Tickets consolidation
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Helloworld Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Helloworld Travel, probed live across 9 host(s) and 6 registrable domain(s). 9 host(s) serve HTTPS (up to TLSv1.3); 8 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Helloworld Travel
provider_slug: helloworld-travel
slug: helloworld-travel-domain-security
source_filename: helloworld-travel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Helloworld Travel Limited web and trade host\nsummary: >-\n  Every Helloworld host probed negotiates TLS 1.3 and every one except expresstickets.com.au\n  returns HSTS with a one-year max-age. Email authentication is uneven across the estate: the\n  four brand domains that sit in front of travellers and agents (helloworld.com.au,\n  readyrooms.com.au, airtickets.com.au, expresstickets.com.au) all publish SPF and a delegated\n  DMARC record at p=reject via EasyDMARC, while the corporate domain helloworldlimited.com.au\n  publishes SPF but NO DMARC at all, and aotonline.net — the inbound trade booking engine —\n  publishes neither SPF nor DMARC. No domain in the estate is DNSSEC-signed. CAA is published\n  on three of six domains. Absence of a record is recorded here as data, not as an error.\nhosts:\n- host: www.helloworldlimited.com.au\n  role: corporate website\n  http_status: 200\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:43:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: policies.helloworldlimited.com.au\n  role: privacy and cookie policy host\n  http_status: 200\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:43:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.helloworld.com.au\n  role: consumer website (redirects to /Find-Your-Agent.html)\n  http_status: 301\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.readyrooms.com.au\n  role: ReadyRooms B2B hotel and activity booking, agent login\n  http_status: 200\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: covered by the wildcard certificate *.readyrooms.com.au\n- host: athena.readyrooms.com.au\n  role: ReadyRooms agent login application\n  http_status: 200\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Oct  6 06:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.readyrooms.com.au\n  role: provisioned but gated developer host\n  http_status: 401\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:04:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    HTTP Basic on every path (WWW-Authenticate: Basic realm=\"Access is permitted to authorized\n    users\"). HSTS is served on the 401 response itself.\n- host: www.aotonline.net\n  role: AOTonline.net inbound trade booking engine, agency-code login\n  http_status: 302\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:14:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.airtickets.com.au\n  role: Air Tickets / SmartTickets consolidation, agent login\n  http_status: 200\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:12:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: host returns HTTP 200 with an empty\
  \ body for every unknown path (soft 404)\n- host: expresstickets.com.au\n  role: Express Tickets consolidation\n  http_status: 403\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:59:20 2026 GMT\n  hsts: false\n  note: >-\n    Edge returns 403 to a scripted client on every path; no Strict-Transport-Security header was\n    present on that response.\ndomains:\n- domain: helloworldlimited.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:zoho.com ~all\n  dmarc: false\n  note: corporate domain publishes SPF with a soft fail and no DMARC record\n- domain: helloworld.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.helloworld_com_au._d.easydmarc.pro -all\n  dmarc: true\n  dmarc_delegated: true\n  dmarc_policy: reject\n  dmarc_pct:\
  \ 100\n- domain: readyrooms.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.readyrooms_com_au._d.easydmarc.pro ~all\n  dmarc: true\n  dmarc_delegated: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  note: DMARC aggregate and forensic reporting is split between EasyDMARC and Proofpoint\n- domain: aotonline.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: false\n  dmarc: false\n  note: the inbound trade booking domain publishes neither SPF nor DMARC\n- domain: airtickets.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.airtickets_com_au._d.easydmarc.pro -all\n  dmarc: true\n  dmarc_delegated: true\n  dmarc_policy:\
  \ reject\n  dmarc_pct: 100\n- domain: expresstickets.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.expresstickets_com_au._d.easydmarc.pro -all\n  dmarc: true\n  dmarc_delegated: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helloworld-travel/refs/heads/main/security/helloworld-travel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- New Zealand
- Travel Agency
- Distribution
- Corporate Travel
- Wholesale
- Hotels
- Booking
- Air Consolidation
- Inbound Tourism
- Tour Operator
---
