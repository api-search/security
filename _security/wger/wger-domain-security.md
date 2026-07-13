---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wger.de
  spf: true
hosts:
- cert_expires: Aug 14 17:50:21 2026 GMT
  host: wger.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wger
provider_slug: wger
slug: wger-domain-security
source_filename: wger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wger.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:50:21 2026 GMT\n  hsts: false\ndomains:\n- domain: wger.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wger/refs/heads/main/security/wger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports And Fitness
- Public APIs
---
