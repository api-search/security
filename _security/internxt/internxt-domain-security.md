---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: internxt.com
  spf: true
hosts:
- cert_expires: Jan 17 05:03:46 2027 GMT
  host: internxt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Internxt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internxt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Internxt
provider_slug: internxt
slug: internxt-domain-security
source_filename: internxt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: internxt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 05:03:46 2027 GMT\n  hsts: null\ndomains:\n- domain: internxt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/internxt/security/internxt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Storage
- Encryption
- Privacy
- Europe
---
