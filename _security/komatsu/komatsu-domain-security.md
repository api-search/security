---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: komatsu.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.komatsu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Komatsu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Komatsu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Komatsu
provider_slug: komatsu
slug: komatsu-domain-security
source_filename: komatsu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.komatsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: komatsu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/komatsu/security/komatsu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Mining
- Industrial Equipment
- Heavy Machinery
---
