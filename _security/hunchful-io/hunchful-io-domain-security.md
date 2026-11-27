---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hunchful.io
  spf: true
hosts:
- cert_expires: Jan 24 11:29:43 2027 GMT
  host: hunchful.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hunchful Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hunchful, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hunchful
provider_slug: hunchful-io
slug: hunchful-io-domain-security
source_filename: hunchful-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hunchful.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 11:29:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: hunchful.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hunchful-io/security/hunchful-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Family
- Calendar
- Artificial Intelligence
- Productivity
- Sweden
---
