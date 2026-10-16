---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: svt.se
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: svt.se
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Svt Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SVT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SVT
provider_slug: svt-se
slug: svt-se-domain-security
source_filename: svt-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: svt.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: svt.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/svt-se/refs/heads/main/security/svt-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Public Service
- Television
- Sweden
- News
---
