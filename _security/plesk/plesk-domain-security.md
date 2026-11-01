---
api_specs:
- filename: plesk-openapi-generated.yml
  format: yaml
  label: Plesk API
  slug: plesk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plesk/openapi/_ae-authored/plesk-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plesk.com
  spf: true
hosts:
- cert_expires: Jan 18 15:52:59 2027 GMT
  host: plesk.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Plesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plesk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plesk
provider_slug: plesk
slug: plesk-domain-security
source_filename: plesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 15:52:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: plesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/plesk/security/plesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web Hosting
- Server Management
- Control Panel
- Automation
- WordPress
---
