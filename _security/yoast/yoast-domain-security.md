---
api_specs:
- filename: yoast-rest-openapi.yml
  format: yaml
  label: Yoast REST API
  slug: yoast-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-rest-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yoast.com
  spf: true
hosts:
- cert_expires: Sep 18 14:43:29 2026 GMT
  host: yoast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 01:47:04 2026 GMT
  host: developer.yoast.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yoast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoast, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yoast
provider_slug: yoast
slug: yoast-domain-security
source_filename: yoast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:43:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.yoast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:47:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yoast.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/security/yoast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- SEO
- WordPress
- Content Optimization
- Schema
- Metadata
---
