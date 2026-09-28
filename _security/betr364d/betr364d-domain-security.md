---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: betr.app
  spf: true
hosts:
- cert_expires: Dec 22 20:32:42 2026 GMT
  host: www.betr.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Betr364D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betr364d, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Betr364d
provider_slug: betr364d
slug: betr364d-domain-security
source_filename: betr364d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betr.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 20:32:42 2026 GMT\n  hsts: false\ndomains:\n- domain: betr.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betr364d/refs/heads/main/security/betr364d-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Gaming
- Sports
- Social
- Betting
- App
- Company
---
