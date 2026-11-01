---
api_specs:
- filename: shotkit-net-openapi-generated.yml
  format: yaml
  label: shotkit-net API
  slug: shotkit-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shotkit-net/openapi/_ae-authored/shotkit-net-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shotkit.net
  spf: true
hosts:
- cert_expires: Jan  6 16:25:55 2027 GMT
  host: shotkit.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Shotkit Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for shotkit-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: shotkit-net
provider_slug: shotkit-net
slug: shotkit-net-domain-security
source_filename: shotkit-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shotkit.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 16:25:55 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: shotkit.net\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/shotkit-net/security/shotkit-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Screenshot
- API
- Web
- Automation
---
