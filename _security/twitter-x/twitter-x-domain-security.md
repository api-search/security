---
api_specs:
- filename: twitter-x-x-api-v2-openapi.json
  format: json
  label: X API v2
  slug: x-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/openapi/twitter-x-x-api-v2-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: x.com
  spf: true
  spf_policy: -all (hard fail); Google, Salesforce, Oracle email delivery included
hosts:
- cert_expires: Aug 26 06:29:58 2026 GMT
  host: x.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:29:58 2026 GMT
  host: api.x.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
- host: docs.x.com
  hsts: true
  hsts_max_age: 63072000
  https: true
- host: developer.x.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 631138519
  https: true
kind: domain-security
layout: security
method: probed
name: Twitter X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Twitter/X, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Twitter/X
provider_slug: twitter-x
slug: twitter-x-domain-security
source_filename: twitter-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, run manually on\n  2026-07-21 (probe-domain-security.py structurally excludes x.com/twitter.com\n  hosts via its social-domain filter, so the identical probes were executed by\n  hand: curl -I for HTTPS/HSTS, openssl s_client for TLS version and cert\n  expiry, dig for DNSKEY/DS/CAA/TXT/_dmarc).\nhosts:\n- host: x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n  hsts_include_subdomains: true\n- host: api.x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:29:58 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\n  hsts_include_subdomains: true\n- host: docs.x.com\n  https: true\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.x.com\n  https: true\n  hsts: true\n  hsts_max_age: 631138519\n  hsts_include_subdomains: true\ndomains:\n- domain: x.com\n  dnssec: false\n\
  \  caa: []\n  spf: true\n  spf_policy: '-all (hard fail); Google, Salesforce, Oracle email delivery included'\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitter-x/refs/heads/main/security/twitter-x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Social Media
- Posts
- Real-Time
- Streaming
- News
- Developer Platform
---
