---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: demisignal.com
  spf: true
hosts:
- cert_expires: Dec 27 10:30:45 2026 GMT
  host: demisignal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Demisignal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DemiSignal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DemiSignal
provider_slug: demisignal-com
slug: demisignal-com-domain-security
source_filename: demisignal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: demisignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:30:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: demisignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/demisignal-com/security/demisignal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Authentication
- DMARC
- SPF
- DKIM
- Email Security
- DNS
- Domain Monitoring
- MCP
---
