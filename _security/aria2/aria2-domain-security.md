---
api_specs:
- filename: aria2-openapi-generated.yml
  format: yaml
  label: aria2 API
  slug: aria2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aria2/openapi/_ae-authored/aria2-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:is-admin@canonical.com"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubuntu.com
  spf: true
hosts:
- cert_expires: Dec 15 04:14:36 2026 GMT
  host: ubuntu.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aria2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aria2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aria2
provider_slug: aria2
slug: aria2-domain-security
source_filename: aria2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubuntu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 04:14:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: ubuntu.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:is-admin@canonical.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v01.api.letsencrypt.org/acme/reg/32541290\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aria2/security/aria2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Download
- OpenSource
- CommandLine
- MultiProtocol
---
