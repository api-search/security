---
api_specs:
- filename: eon-openapi-original.yml
  format: yaml
  label: Eon API
  slug: eon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/openapi/eon-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eon.io
  spf: true
hosts:
- cert_expires: Oct  6 12:24:09 2026 GMT
  host: eon.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eon
provider_slug: eon
slug: eon-domain-security
source_filename: eon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eon.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eon.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon/refs/heads/main/security/eon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Backup
- Data Protection
- Disaster Recovery
- Ransomware Protection
- Backup
- Cloud Storage
- Data Lake
- Multi-Cloud
- Azure
- Google Cloud
---
