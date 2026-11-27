---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openquality.us
  spf: true
hosts:
- cert_expires: Jan 10 21:52:34 2027 GMT
  host: openquality.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Quality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Quality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Quality
provider_slug: openquality-us
slug: openquality-us-domain-security
source_filename: openquality-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openquality.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 21:52:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openquality.us\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openquality-us/security/openquality-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Quality Measures
- Open Source
- FHIR
---
