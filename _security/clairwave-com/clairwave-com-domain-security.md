---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clairwave.com
  spf: true
hosts:
- cert_expires: Jan 31 07:50:45 2027 GMT
  host: clairwave.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clairwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clairwave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clairwave
provider_slug: clairwave-com
slug: clairwave-com-domain-security
source_filename: clairwave-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clairwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 07:50:45 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: clairwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clairwave-com/security/clairwave-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Underwater Acoustics
- marine modeling
- environmental impact assessment
- Offshore Energy
- port and shipping
- AI Integration
---
