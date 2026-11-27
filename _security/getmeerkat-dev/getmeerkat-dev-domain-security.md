---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: getmeerkat.dev
  spf: false
hosts:
- cert_expires: Dec 19 12:02:20 2026 GMT
  host: getmeerkat.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meerkat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meerkat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Meerkat
provider_slug: getmeerkat-dev
slug: getmeerkat-dev-domain-security
source_filename: getmeerkat-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmeerkat.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 12:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getmeerkat.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getmeerkat-dev/security/getmeerkat-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Prompt Engineering
- Platform
- Startups
- Meerkat
---
