---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: quarantine
  dmarc_rua: mailto:dmarc@garten.co
  dnssec: false
  domain: garten.co
  spf: true
  spf_policy: -all
  spf_record: v=spf1 include:_u.garten.co._spf.dmarclc.com include:mail.zendesk.com include:spf.zoho.com include:transmail.net include:_spf.intacct.com -all
hosts:
- cert_expires: Sep  5 19:05:32 2026 GMT
  host: garten.co
  hsts: false
  http_status: 200
  https: true
  note: WordPress corporate site (W3 Total Cache, Yoast)
  tls_version: TLSv1.2
- cert_expires: Sep  5 19:05:32 2026 GMT
  host: www.garten.co
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 14 21:57:47 2026 GMT
  host: tv.garten.co
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
  note: garten TV on the Uscreen platform (Google Frontend); the only host carrying HSTS and the only host with a discovery surface
  tls_version: TLSv1.3
- cert_expires: Sep  5 19:05:32 2026 GMT
  host: api.garten.co
  hsts: false
  http_status: 200
  https: true
  note: Spree/Solidus commerce application; /api/v1 and /api/v2 answer HTTP 401 "You must specify an API key."
  tls_version: TLSv1.2
- cert_expires: Sep  5 19:05:32 2026 GMT
  host: client.garten.co
  hsts: false
  http_status: 200
  https: true
  note: garten client portal — same application as api.garten.co
  tls_version: TLSv1.2
- cert_expires: Sep 23 03:32:12 2026 GMT
  host: experiences.garten.co
  hsts: false
  http_status: 200
  https: true
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: admin.garten.co
  hsts: false
  http_status: 200
  https: true
  note: internal admin tool on AWS Elastic Beanstalk; SPA catch-all returns 200 for every path
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Garten Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Garten, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Garten
provider_slug: garten
slug: garten-domain-security
source_filename: garten-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + discovered garten.co hosts\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py, then extended by hand with the\n  additional garten.co hosts found during contract discovery (DNS + crt.sh). The script\n  reported `hsts: null` for tv.garten.co because of how it reads the root document; a HEAD\n  of https://tv.garten.co/ and a POST to https://tv.garten.co/mcp both return\n  `strict-transport-security: max-age=63072000; includeSubDomains`, so HSTS is recorded\n  true for that host.\nhosts:\n- host: garten.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 19:05:32 2026 GMT\n  hsts: false\n  http_status: 200\n  note: WordPress corporate site (W3 Total Cache, Yoast)\n- host: www.garten.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 19:05:32 2026 GMT\n  hsts: false\n  http_status: 200\n- host: tv.garten.co\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Oct 14 21:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  http_status: 200\n  note: garten TV on the Uscreen platform (Google Frontend); the only host carrying HSTS\n    and the only host with a discovery surface\n- host: api.garten.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 19:05:32 2026 GMT\n  hsts: false\n  http_status: 200\n  note: Spree/Solidus commerce application; /api/v1 and /api/v2 answer HTTP 401 \"You must\n    specify an API key.\"\n- host: client.garten.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 19:05:32 2026 GMT\n  hsts: false\n  http_status: 200\n  note: garten client portal — same application as api.garten.co\n- host: experiences.garten.co\n  https: true\n  cert_expires: Sep 23 03:32:12 2026 GMT\n  hsts: false\n  http_status: 200\n- host: admin.garten.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n  http_status: 200\n\
  \  note: internal admin tool on AWS Elastic Beanstalk; SPA catch-all returns 200 for every\n    path\ndomains:\n- domain: garten.co\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  spf_record: 'v=spf1 include:_u.garten.co._spf.dmarclc.com include:mail.zendesk.com\n    include:spf.zoho.com include:transmail.net include:_spf.intacct.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: mailto:dmarc@garten.co\n  dmarc_pct: 100\nsummary:\n  strengths:\n  - SPF published with a hard fail (-all)\n  - DMARC published at p=quarantine with pct=100 and both rua and ruf reporting\n  - HSTS with a two-year max-age and includeSubDomains on the garten TV host\n  gaps:\n  - no DNSSEC on garten.co\n  - no CAA records, so any CA may issue for the domain\n  - no HSTS on the corporate site, the client portal or the commerce API host, all of\n    which still negotiate at TLS 1.2 rather than TLS 1.3\n  - DMARC policy is quarantine rather than reject\nx-evidence:\n  fetched: '2026-08-04'\n\
  \  tools: [dig, openssl s_client, curl]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/garten/refs/heads/main/security/garten-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Food Service
- Corporate Wellness
- Workplace
- Catering
- Employee Benefits
- Micro Market
- Facilities Management
- Hospitality
- Streaming Video
- MCP
---
