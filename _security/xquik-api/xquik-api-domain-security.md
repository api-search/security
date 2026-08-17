---
api_specs:
- filename: xquik-rest-api-openapi.yml
  format: yaml
  label: Xquik REST API
  slug: xquik-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/openapi/xquik-rest-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: xquik.com
  spf: true
hosts:
- cert_expires: Sep 15 15:19:24 2026 GMT
  host: xquik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 08:49:03 2026 GMT
  host: docs.xquik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xquik Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xquik, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Xquik
provider_slug: xquik-api
slug: xquik-api-domain-security
source_filename: xquik-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xquik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:19:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.xquik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 08:49:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: xquik.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xquik-api/refs/heads/main/security/xquik-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- social media data
- X / Twitter
- social listening
- data extraction
- automation
- webhooks
- MCP
- developer API
---
