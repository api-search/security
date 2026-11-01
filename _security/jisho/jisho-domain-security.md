---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  dmarc: false
  dnssec: false
  domain: jisho.org
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: jisho.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jisho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jisho.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jisho.org
provider_slug: jisho
slug: jisho-domain-security
source_filename: jisho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jisho.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jisho.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/jisho/security/jisho-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Japanese
- Dictionary
- Language-Learning
- API
---
