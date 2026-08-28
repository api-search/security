---
api_specs:
- filename: silent-push-web-scanner.postman_collection.json
  format: json
  label: Silent Push API
  slug: silent-push-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/postman/silent-push-web-scanner.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silentpush.com
  spf: true
hosts:
- cert_expires: Oct 18 18:14:58 2026 GMT
  host: www.silentpush.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:36:25 2026 GMT
  host: help.silentpush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: api.silentpush.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: mcp.silentpush.com
  hsts: false
  https: true
  note: MCP endpoint host; probed 2026-08-27, no Strict-Transport-Security header on the 401 challenge
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: explore.silentpush.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silent Push Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silent Push, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Silent Push
provider_slug: silent-push
slug: silent-push-domain-security
source_filename: silent-push-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silentpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:14:58 2026 GMT\n  hsts: false\n- host: help.silentpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.silentpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.silentpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: false\n  note: MCP endpoint host; probed 2026-08-27, no Strict-Transport-Security header on the 401 challenge\n- host: explore.silentpush.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: silentpush.com\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silent-push/refs/heads/main/security/silent-push-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- DNS
- Domain Intelligence
- Passive DNS
- Enrichment
- Threat Feeds
- WHOIS
- Model Context Protocol
---
