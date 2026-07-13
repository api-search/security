---
api_specs:
- filename: discourse-openapi.json
  format: json
  label: Discourse API
  slug: discourse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/openapi/discourse-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: discourse.org
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.discourse.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:02:48 2026 GMT
  host: meta.discourse.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discourse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Discourse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Discourse
provider_slug: discourse
slug: discourse-domain-security
source_filename: discourse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.discourse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: meta.discourse.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:02:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: discourse.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discourse/refs/heads/main/security/discourse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communities
- Forums
- Open Source
---
