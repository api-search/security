---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_rua: mailto:dmarc-reports@theblueground.com
  dnssec: true
  domain: theblueground.com
  spf: true
  spf_policy: ~all
hosts:
- cert_expires: Oct 11 14:42:19 2026 GMT
  host: www.theblueground.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 14:42:19 2026 GMT
  host: api.theblueground.com
  hsts: false
  http_status: 404
  https: true
  note: Live Go service; answers `404 page not found` (text/plain) on every path probed.
  tls_version: TLSv1.3
- cert_expires: Oct 11 14:42:19 2026 GMT
  host: partner-network.theblueground.com
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 15:14:09 2026 GMT
  host: partners.theblueground.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: cdn.theblueground.com
  hsts: false
  http_status: 403
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blueground Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blueground, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blueground
provider_slug: blueground
slug: blueground-domain-security
source_filename: blueground-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py, then extended by hand with the\n  additional Blueground hosts probed during contract discovery. The script reported\n  `spf: false` because theblueground.com publishes its SPF policy as a MULTI-STRING TXT\n  record; `dig +short TXT theblueground.com` confirms `v=spf1 include:eu.transmail.net\n  include:mail.zendesk.com include:_spf.google.com include:_spf.salesforce.com\n  include:aspmx.pardot.com ... ~all`, so spf is recorded true here.\nhosts:\n- host: www.theblueground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:42:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.theblueground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:42:19 2026 GMT\n  hsts: false\n  http_status: 404\n  note: Live Go service; answers `404 page not found` (text/plain) on every path\
  \ probed.\n- host: partner-network.theblueground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:42:19 2026 GMT\n  hsts: false\n  http_status: 200\n- host: partners.theblueground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 15:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  http_status: 200\n- host: cdn.theblueground.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n  http_status: 403\ndomains:\n- domain: theblueground.com\n  dnssec: true\n  caa: []\n  spf: true\n  spf_policy: '~all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_rua: mailto:dmarc-reports@theblueground.com\nx-evidence:\n  fetched: '2026-07-31'\n  tools: [dig, openssl s_client, curl]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blueground/refs/heads/main/security/blueground-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Real-Estate
- PropTech
- Travel
- Hospitality
- Furnished Rentals
- Property Management
- Corporate Housing
- Marketplace
---
