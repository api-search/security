---
api_specs:
- filename: backblaze-b2-native-api.yaml
  format: yaml
  label: Backblaze B2 Cloud Storage API
  slug: backblaze-b2-cloud-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/openapi/backblaze-b2-native-api.yaml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: backblaze.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: backblazeb2.com
  spf: true
hosts:
- cert_expires: Oct  7 21:09:01 2026 GMT
  host: www.backblaze.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 19:08:51 2026 GMT
  host: api.backblazeb2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backblaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backblaze, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Backblaze
provider_slug: backblaze
slug: backblaze-domain-security
source_filename: backblaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backblaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:09:01 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.backblazeb2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:08:51 2026 GMT\n  hsts: null\ndomains:\n- domain: backblaze.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: backblazeb2.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backblaze/refs/heads/main/security/backblaze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
---
