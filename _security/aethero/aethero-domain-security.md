---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aethero.com
  spf: true
hosts:
- cert_expires: Jan  1 11:36:00 2027 GMT
  host: aethero.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Aethero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aethero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aethero
provider_slug: aethero
slug: aethero-domain-security
source_filename: aethero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aethero.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 11:36:00 2027 GMT\n  hsts: false\ndomains:\n- domain: aethero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aethero/refs/heads/main/security/aethero-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Space
- Edge Computing
- Satellites
- Artificial Intelligence
- Machine Learning
- Aerospace
- Defense
- Hardware
---
