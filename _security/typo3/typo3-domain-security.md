---
api_specs:
- filename: typo3-releases-openapi.json
  format: json
  label: TYPO3 Releases REST API
  slug: releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/openapi/typo3-releases-openapi.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:admin@typo3.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: typo3.org
  spf: true
hosts:
- cert_expires: Oct  7 05:03:04 2026 GMT
  host: typo3.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 06:28:10 2026 GMT
  host: docs.typo3.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: example.typo3.org
  https: false
kind: domain-security
layout: security
method: probed
name: Typo3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TYPO3, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TYPO3
provider_slug: typo3
slug: typo3-domain-security
source_filename: typo3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: typo3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 05:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.typo3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 06:28:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: example.typo3.org\n  https: false\ndomains:\n- domain: typo3.org\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:admin@typo3.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/security/typo3-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CMS
- Content Management
- Enterprise
- PHP
- Headless
- JSON API
- Open Source
---
