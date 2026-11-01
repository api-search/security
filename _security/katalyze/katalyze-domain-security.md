---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: katalyzeai.com
  spf: true
hosts:
- cert_expires: Jan  7 20:26:48 2027 GMT
  host: katalyzeai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Katalyze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Katalyze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Katalyze
provider_slug: katalyze
slug: katalyze-domain-security
source_filename: katalyze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katalyzeai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 20:26:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: katalyzeai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/katalyze/security/katalyze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Life Sciences
- GxP
- Deviation Investigation
- Yield Optimization
- Raw Material Characterization
- Tech Transfer
- Document Intelligence
---
