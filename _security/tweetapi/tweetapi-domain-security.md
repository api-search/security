---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tweetapi.com
  spf: true
hosts:
- cert_expires: Nov  3 15:00:35 2026 GMT
  host: tweetapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 09:40:40 2026 GMT
  host: api.tweetapi.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 15:42:10 2026 GMT
  host: mcp.tweetapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tweetapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TweetAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TweetAPI
provider_slug: tweetapi
slug: tweetapi-domain-security
source_filename: tweetapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tweetapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 15:00:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tweetapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 09:40:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: mcp.tweetapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:42:10 2026 GMT\n  hsts: null\ndomains:\n- domain: tweetapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweetapi/refs/heads/main/security/tweetapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Twitter
- x
- social-media
- social-data
- Search
- Analytics
- research
- Developer Tools
- MCP
- agent-native
- llms-txt
- REST API
---
