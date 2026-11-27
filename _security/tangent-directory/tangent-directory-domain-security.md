---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tangent.directory
  spf: true
hosts:
- cert_expires: Dec 31 10:44:46 2026 GMT
  host: tangent.directory
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tangent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tangent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tangent
provider_slug: tangent-directory
slug: tangent-directory-domain-security
source_filename: tangent-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tangent.directory\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 10:44:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tangent.directory\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tangent-directory/security/tangent-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Inspiration
- UI
- Community
- Resources
---
