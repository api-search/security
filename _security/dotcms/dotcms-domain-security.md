---
api_specs:
- filename: dotcms-openapi.yml
  format: yaml
  label: dotCMS REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/openapi/dotcms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dotcms.com
  spf: true
hosts:
- cert_expires: Sep 30 21:45:31 2026 GMT
  host: dev.dotcms.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 00:51:21 2026 GMT
  host: demo.dotcms.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dotcms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dotCMS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dotCMS
provider_slug: dotcms
slug: dotcms-domain-security
source_filename: dotcms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.dotcms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.dotcms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:51:21 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: dotcms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotcms/refs/heads/main/security/dotcms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content
- Content Management
---
