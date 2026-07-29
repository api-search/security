---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wyndhamhotels.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wyndhambusiness.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  edge: Akamai
  host: www.wyndhamhotels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 13 15:40:32 2026 GMT
  host: corporate.wyndhamhotels.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 22:56:31 2026 GMT
  host: development.wyndhamhotels.com
  hsts: false
  https: true
  note: WordPress on WP Engine; anonymous WordPress REST API and a gated MCP adapter.
  tls_version: TLSv1.3
- cert_expires: Oct 12 08:02:03 2026 GMT
  host: investor.wyndhamhotels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: mcp.wyndhamhotels.com
  hsts: null
  https: true
  note: Provisioned behind Akamai; every path returns 503 with no HSTS header.
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: aisearch.wyndhamhotels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 03:31:55 2026 GMT
  host: connect.wyndhamhotels.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Returns HTTP 204 with an empty body on every path.
  tls_version: TLSv1.3
- cert_expires: Oct 18 21:51:59 2026 GMT
  edge: Cloudflare (WP Engine origin)
  host: www.wyndhambusiness.com
  hsts: false
  https: true
  note: 'Carries the only live, machine-readable API surfaces on the estate — an

    anonymous WordPress REST API and an OAuth 2.1 protected MCP server — and is one

    of the hosts with no HSTS.

    '
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wyndham Hotels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wyndham Hotels & Resorts, probed live across 8 host(s) and 2 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.2); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wyndham Hotels & Resorts
provider_slug: wyndham-hotels
slug: wyndham-hotels-domain-security
source_filename: wyndham-hotels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every Wyndham host named in apis.yml, review.yml\n  and the harvested discovery documents\nhosts:\n- host: www.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  edge: Akamai\n- host: corporate.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:40:32 2026 GMT\n  hsts: false\n- host: development.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:56:31 2026 GMT\n  hsts: false\n  note: WordPress on WP Engine; anonymous WordPress REST API and a gated MCP adapter.\n- host: investor.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 08:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n  note:\
  \ Provisioned behind Akamai; every path returns 503 with no HSTS header.\n- host: aisearch.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.wyndhamhotels.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 03:31:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Returns HTTP 204 with an empty body on every path.\n- host: www.wyndhambusiness.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 21:51:59 2026 GMT\n  hsts: false\n  edge: Cloudflare (WP Engine origin)\n  note: |\n    Carries the only live, machine-readable API surfaces on the estate — an\n    anonymous WordPress REST API and an OAuth 2.1 protected MCP server — and is one\n    of the hosts with no HSTS.\ndomains:\n- domain: wyndhamhotels.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wyndhambusiness.com\n  dnssec: false\n  caa: []\n \
  \ spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n  no_caa: |\n    Neither registrable domain publishes a CAA record, so no certificate authority is\n    pinned for either estate.\n  no_dnssec: Neither domain is DNSSEC-signed.\n  hsts_gaps:\n  - corporate.wyndhamhotels.com\n  - development.wyndhamhotels.com\n  - www.wyndhambusiness.com\n  tls_note: |\n    www.wyndhamhotels.com negotiates TLS 1.2 while every other host negotiates\n    TLS 1.3.\n  dmarc_note: |\n    wyndhamhotels.com enforces p=reject; wyndhambusiness.com only p=quarantine.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyndham-hotels/refs/heads/main/security/wyndham-hotels-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Franchising
- Distribution
- Loyalty
- GDS
---
