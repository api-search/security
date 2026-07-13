---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joomla.org
  spf: true
hosts:
- cert_expires: Sep 22 06:59:19 2026 GMT
  host: www.joomla.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 06:59:19 2026 GMT
  host: docs.joomla.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Joomla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joomla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Joomla
provider_slug: joomla
slug: joomla-domain-security
source_filename: joomla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joomla.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:59:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joomla.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 06:59:19 2026 GMT\n  hsts: null\ndomains:\n- domain: joomla.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/joomla/refs/heads/main/security/joomla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Open Source
- PHP
- REST API
- Articles
- Categories
- Contacts
- Menus
- Modules
- Users
---
