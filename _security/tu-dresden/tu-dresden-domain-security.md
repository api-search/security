---
api_specs:
- filename: tu-dresden-slub-lod.yaml
  format: yaml
  label: SLUB Dresden Linked Open Data API
  slug: slub-lod
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/openapi/tu-dresden-slub-lod.yaml
description: ''
domains:
- caa:
  - 0 issuewild ";"
  - 0 iodef "mailto:ca@tu-dresden.de"
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tu-dresden.de
  spf: true
hosts:
- cert_expires: Oct 28 16:20:14 2026 GMT
  host: tu-dresden.de
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 05:08:25 2026 GMT
  host: vvz.phil.tu-dresden.de
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:12:47 2027 GMT
  host: idp.tu-dresden.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tu Dresden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TU Dresden, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TU Dresden
provider_slug: tu-dresden
slug: tu-dresden-domain-security
source_filename: tu-dresden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tu-dresden.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:20:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: vvz.phil.tu-dresden.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:08:25 2026 GMT\n  hsts: false\n- host: idp.tu-dresden.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:12:47 2027 GMT\n  hsts: false\ndomains:\n- domain: tu-dresden.de\n  dnssec: false\n  caa:\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:ca@tu-dresden.de\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/security/tu-dresden-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Germany
---
