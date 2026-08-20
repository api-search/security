---
api_specs:
- filename: medialab-ai-imgur-api.postman_collection.json
  format: json
  label: Imgur API
  slug: imgur-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/postman/medialab-ai-imgur-api.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medialab.la
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genius.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imgur.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: medialab.la
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 01:40:34 2026 GMT
  host: docs.genius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 01:40:34 2026 GMT
  host: api.genius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 10 01:40:34 2026 GMT
  host: genius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.imgur.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 13 14:52:36 2026 GMT
  host: apidocs.imgur.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: imgur.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Medialab Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MediaLab.AI, probed live across 8 host(s) and 4 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MediaLab.AI
provider_slug: medialab-ai
slug: medialab-ai-domain-security
source_filename: medialab-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medialab.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 01:40:34 2026 GMT\n  hsts: false\n- host: api.genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 01:40:34 2026 GMT\n  hsts: false\n- host: genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 01:40:34 2026 GMT\n  hsts: false\n- host: api.imgur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\n- host: apidocs.imgur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 14:52:36 2026 GMT\n  hsts:\
  \ true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  hsts_include_subdomains: true\n- host: imgur.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: medialab.la\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: genius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: imgur.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: Corporate hosts probed by 0-working/probe-domain-security.py; the Genius and\n  Imgur API/doc hosts were probed manually (same TLS/HSTS/DNS method) because the\n  portfolio brand domains are not reachable from medialab.la in apis.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medialab-ai/refs/heads/main/security/medialab-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Social
- Advertising
- Content
- Image
- Music
- Messaging
- Communities
- Holding Company
---
