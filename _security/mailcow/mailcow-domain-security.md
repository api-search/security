---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: mailcow.email
  spf: true
hosts:
- cert_expires: Jan 22 23:38:22 2027 GMT
  host: mailcow.email
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailcow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mailcow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: mailcow
provider_slug: mailcow
slug: mailcow-domain-security
source_filename: mailcow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailcow.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:38:22 2027 GMT\n  hsts: false\ndomains:\n- domain: mailcow.email\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mailcow/security/mailcow-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Email
- Docker
- OpenSource
- SelfHosted
---
