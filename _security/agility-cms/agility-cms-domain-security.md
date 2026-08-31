---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agilitycms.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: aglty.io
  spf: false
hosts:
- cert_expires: Sep 18 05:44:10 2026 GMT
  host: agilitycms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 09:33:31 2026 GMT
  host: api.aglty.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agility Cms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agility CMS, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agility CMS
provider_slug: agility-cms
slug: agility-cms-domain-security
source_filename: agility-cms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agilitycms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 05:44:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aglty.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agilitycms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aglty.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agility-cms/refs/heads/main/security/agility-cms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Headless CMS
- Content Management
- REST
- Multi-site
---
