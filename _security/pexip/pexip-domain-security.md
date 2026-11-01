---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pexip.com
  spf: true
hosts:
- cert_expires: Jan 15 20:29:54 2027 GMT
  host: pexip.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pexip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pexip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pexip
provider_slug: pexip
slug: pexip-domain-security
source_filename: pexip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pexip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 20:29:54 2027 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: pexip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/pexip/security/pexip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Video
- Communications
- Cloud
- Security
- Enterprise
---
