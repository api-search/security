---
api_specs:
- filename: backupify-saas-protection-api.yaml
  format: yaml
  label: Backupify SaaS Protection API
  slug: saas-protection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/openapi/backupify-saas-protection-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: backupify.com
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issue "Digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dattobackup.com
  spf: true
hosts:
- cert_expires: Aug 18 23:55:46 2026 GMT
  host: www.backupify.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: portal.dattobackup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 00:54:57 2026 GMT
  host: api.datto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backupify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backupify, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Backupify
provider_slug: backupify
slug: backupify-domain-security
source_filename: backupify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.backupify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:55:46 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: portal.dattobackup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.datto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:54:57 2026 GMT\n  hsts: null\ndomains:\n- domain: backupify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dattobackup.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"Digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backupify/refs/heads/main/security/backupify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Backup
- Data Protection
- Cloud Backup
- Microsoft 365
- Google Workspace
---
