---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: silverstripe.org
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.silverstripe.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 01:23:52 2026 GMT
  host: docs.silverstripe.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silverstripe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SilverStripe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SilverStripe
provider_slug: silverstripe
slug: silverstripe-domain-security
source_filename: silverstripe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silverstripe.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\n- host: docs.silverstripe.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 01:23:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: silverstripe.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silverstripe/refs/heads/main/security/silverstripe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- GraphQL
- REST API
- PHP
- Open Source
- Framework
- Pages
- Assets
- Versioning
---
