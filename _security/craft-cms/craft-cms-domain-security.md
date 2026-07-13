---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: craftcms.com
  spf: true
hosts:
- cert_expires: Sep  6 00:41:05 2026 GMT
  host: craftcms.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: example.craftcms.com
  https: false
kind: domain-security
layout: security
method: probed
name: Craft Cms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craft CMS, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Craft CMS
provider_slug: craft-cms
slug: craft-cms-domain-security
source_filename: craft-cms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftcms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:41:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: example.craftcms.com\n  https: false\ndomains:\n- domain: craftcms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craft-cms/refs/heads/main/security/craft-cms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- GraphQL
- REST
- Headless
- PHP
---
