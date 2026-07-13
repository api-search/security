---
api_specs:
- filename: imgix-openapi.yml
  format: yaml
  label: Imgix Rendering API
  slug: imgix-rendering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imgix/refs/heads/main/openapi/imgix-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issue "entrust.net"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: imgix.com
  spf: true
hosts:
- cert_expires: Aug 17 08:36:44 2026 GMT
  host: imgix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 09:20:57 2026 GMT
  host: docs.imgix.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:52:38 2026 GMT
  host: api.imgix.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imgix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imgix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Imgix
provider_slug: imgix
slug: imgix-domain-security
source_filename: imgix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imgix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 08:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.imgix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:20:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.imgix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:52:38 2026 GMT\n  hsts: null\ndomains:\n- domain: imgix.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"entrust.net\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imgix/refs/heads/main/security/imgix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDN
- Image Optimization
- Image Processing
- Media
---
