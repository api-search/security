---
api_specs:
- filename: duplicati-default-api-openapi.yml
  format: yaml
  label: Duplicati API
  slug: duplicati-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duplicati/openapi/duplicati-default-api-openapi.yml
- filename: duplicati-openapi-generated.yml
  format: yaml
  label: Duplicati API
  slug: duplicati-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duplicati/openapi/_ae-authored/duplicati-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: duplicati.com
  spf: true
hosts:
- cert_expires: Dec  9 21:56:15 2026 GMT
  host: duplicati.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Duplicati Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duplicati, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Duplicati
provider_slug: duplicati
slug: duplicati-domain-security
source_filename: duplicati-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duplicati.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 21:56:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: duplicati.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/duplicati/security/duplicati-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Backup
- Open-Source
- Cloud
- Security
---
