---
api_specs:
- filename: wix-openapi.yml
  format: yaml
  label: Wix REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-openapi.yml
- filename: wix-asyncapi.yml
  format: yaml
  label: Wix Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/asyncapi/wix-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wixapis.com
  spf: false
hosts:
- cert_expires: Sep 12 11:54:01 2026 GMT
  host: www.wix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 11:54:01 2026 GMT
  host: dev.wix.com
  hsts: true
  hsts_max_age: 120
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:14:54 2026 GMT
  host: www.wixapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wix, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wix
provider_slug: wix
slug: wix-domain-security
source_filename: wix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.wix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 120\n- host: www.wixapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:14:54 2026 GMT\n  hsts: null\ndomains:\n- domain: wix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wixapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/security/wix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- eCommerce
- Headless
- Website Builder
---
