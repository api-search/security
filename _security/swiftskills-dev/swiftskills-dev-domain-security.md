---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swiftskills.dev
  spf: false
hosts:
- cert_expires: Jan 14 07:20:02 2027 GMT
  host: swiftskills.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swiftskills Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for swiftskills-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: swiftskills-dev
provider_slug: swiftskills-dev
slug: swiftskills-dev-domain-security
source_filename: swiftskills-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swiftskills.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 07:20:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: swiftskills.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/swiftskills-dev/security/swiftskills-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Apple
- iOS
- Swift
- Development
---
