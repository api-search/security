---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eslahoradelaverdad.es
  spf: false
hosts:
- cert_expires: Jan  4 18:25:40 2027 GMT
  host: eslahoradelaverdad.es
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eslahoradelaverdad-es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eslahoradelaverdad-es, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: eslahoradelaverdad-es
provider_slug: eslahoradelaverdad-es
slug: eslahoradelaverdad-es-domain-security
source_filename: eslahoradelaverdad-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eslahoradelaverdad.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 18:25:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eslahoradelaverdad.es\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eslahoradelaverdad-es/security/eslahoradelaverdad-es-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
