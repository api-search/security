---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: idea-launch.io
  spf: false
hosts:
- cert_expires: Dec 24 05:51:30 2026 GMT
  host: idea-launch.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Idea Launch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Idea Launch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Idea Launch
provider_slug: idea-launch-io
slug: idea-launch-io-domain-security
source_filename: idea-launch-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idea-launch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 05:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: idea-launch.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/idea-launch-io/security/idea-launch-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Software-as-a-Service
- Marketing
- Validation
- Startups
- Advertising
---
