---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kandou.ai
  spf: true
hosts:
- cert_expires: Oct 14 07:37:13 2026 GMT
  host: www.kandou.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kandou Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kandou, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kandou
provider_slug: kandou
slug: kandou-domain-security
source_filename: kandou-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kandou.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:37:13 2026 GMT\n  hsts: null\ndomains:\n- domain: kandou.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kandou/refs/heads/main/security/kandou-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Semiconductors
- Hardware
- Chiplets
- Interconnect
- SerDes
- AI Infrastructure
- Deep Tech
---
