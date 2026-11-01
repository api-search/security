---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maytech.net
  spf: true
hosts:
- cert_expires: Jan  3 18:24:23 2027 GMT
  host: maytech.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quatrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quatrix (Maytech), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quatrix (Maytech)
provider_slug: quatrix
slug: quatrix-domain-security
source_filename: quatrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maytech.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 18:24:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maytech.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/quatrix/security/quatrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FileTransfer
- SecureData
- Enterprise
- Compliance
- Cloud
---
