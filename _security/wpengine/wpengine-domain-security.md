---
api_specs:
- filename: reference
  format: yaml
  label: WP Engine Hosting Platform API
  slug: wpengine-hosting-platform-api
  spec_type: OpenAPI
  url: https://developers.wpengine.com/docs/managed-hosting-platform/api/reference
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wpengine.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wpengineapi.com
  spf: false
hosts:
- cert_expires: Oct  7 02:08:09 2026 GMT
  host: wpengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 06:04:18 2026 GMT
  host: developers.wpengine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.wpengineapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wpengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WP Engine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WP Engine
provider_slug: wpengine
slug: wpengine-domain-security
source_filename: wpengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wpengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:08:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.wpengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:04:18 2026 GMT\n  hsts: false\n- host: api.wpengineapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wpengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wpengineapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/security/wpengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WordPress
- Managed Hosting
- WordPress Hosting
- Site Management
- Digital Experience Platform
---
