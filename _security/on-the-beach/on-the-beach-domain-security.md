---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: onthebeachgroupplc.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onthebeach.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sunshine.co.uk
  spf: true
hosts:
- cert_expires: Jan 23 19:52:37 2027 GMT
  host: www.onthebeachgroupplc.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:29:09 2026 GMT
  host: www.onthebeach.co.uk
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: HSTS observed on the HTTP/2 response to /.well-known/apple-app-site-association; a plain HEAD of / is answered by the Cloudflare bot challenge.
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:58:37 2026 GMT
  host: www.sunshine.co.uk
  hsts: null
  https: true
  note: HEAD / returns the Cloudflare bot challenge (403); HSTS not observable.
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:29:09 2026 GMT
  cert_issuer: Google Trust Services WE1
  cert_san:
  - onthebeach.co.uk
  - '*.onthebeach.co.uk'
  - '*.staging.onthebeach.co.uk'
  cert_subject: CN=onthebeach.co.uk
  host: mcp.onthebeach.co.uk
  hsts: null
  https: true
  note: 'Deliberate DNS record (no wildcard: foo/chat/agent/ai/api.onthebeach.co.uk are NXDOMAIN). All requests answered by the Cloudflare WAF with 403.'
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:43:23 2026 GMT
  host: help.onthebeach.co.uk
  hsts: true
  hsts_max_age: 259200
  https: true
  note: CNAME onthebeachuk.zendesk.com — Zendesk-hosted help centre.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: On The Beach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for On the Beach, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: On the Beach
provider_slug: on-the-beach
slug: on-the-beach-domain-security
source_filename: on-the-beach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the consumer, help and\n  mcp hosts found during contract discovery\nhosts:\n- host: www.onthebeachgroupplc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 19:52:37 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.onthebeach.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:29:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    HSTS observed on the HTTP/2 response to\n    /.well-known/apple-app-site-association; a plain HEAD of / is answered by\n    the Cloudflare bot challenge.\n- host: www.sunshine.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:58:37 2026 GMT\n  hsts: null\n  note: HEAD / returns the Cloudflare bot challenge (403); HSTS not observable.\n- host: mcp.onthebeach.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:29:09\
  \ 2026 GMT\n  hsts: null\n  cert_subject: CN=onthebeach.co.uk\n  cert_issuer: Google Trust Services WE1\n  cert_san: [onthebeach.co.uk, '*.onthebeach.co.uk', '*.staging.onthebeach.co.uk']\n  note: >-\n    Deliberate DNS record (no wildcard: foo/chat/agent/ai/api.onthebeach.co.uk\n    are NXDOMAIN). All requests answered by the Cloudflare WAF with 403.\n- host: help.onthebeach.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:43:23 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  note: CNAME onthebeachuk.zendesk.com — Zendesk-hosted help centre.\ndomains:\n- domain: onthebeachgroupplc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: onthebeach.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sunshine.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n  positives:\n  - TLS 1.3 on every reachable host\n  - HSTS with a one-year max-age and includeSubDomains\
  \ on the consumer booking host\n  - SPF on all three registrable domains; DMARC enforced on both consumer domains\n    (quarantine on onthebeach.co.uk, reject on sunshine.co.uk)\n  gaps:\n  - No DNSSEC on any domain\n  - No CAA records on any domain\n  - No DMARC record on the corporate/investor domain onthebeachgroupplc.com\n  - No security.txt on any host, and no vulnerability disclosure or trust-center\n    page was found by probe (see review.yml)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/on-the-beach/refs/heads/main/security/on-the-beach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United Kingdom
- OTA
- Online Travel Agency
- Booking
- Package Holidays
- Aviation
- Airline
- Distribution
- NDC
- Hotels
- Hospitality
- MCP
- Artificial Intelligence
---
