---
api_specs:
- filename: jellypod-com-api-openapi.json
  format: json
  label: Jellypod API API
  slug: jellypod-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jellypod-com/openapi/_original/jellypod-com-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jellypod.com
  spf: true
hosts:
- cert_expires: Jan  4 13:14:11 2027 GMT
  host: jellypod.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jellypod, Inc. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jellypod, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jellypod, Inc.
provider_slug: jellypod-com
slug: jellypod-com-domain-security
source_filename: jellypod-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jellypod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 13:14:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jellypod.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jellypod-com/security/jellypod-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcast creation
- Content Automation
- Enterprise content platform
---
