---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aomni.com
  spf: true
hosts:
- cert_expires: Dec 16 12:13:09 2026 GMT
  host: aomni.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aomni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aomni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aomni
provider_slug: aomni
slug: aomni-domain-security
source_filename: aomni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aomni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 12:13:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aomni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aomni/security/aomni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
