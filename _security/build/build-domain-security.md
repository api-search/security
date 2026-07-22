---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: build.inc
  spf: true
hosts:
- cert_expires: Sep 20 02:55:32 2026 GMT
  host: build.inc
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Build Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Build, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Build
provider_slug: build
slug: build-domain-security
source_filename: build-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: build.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:55:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: build.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/build/refs/heads/main/security/build-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business Applications
- Artificial Intelligence
- AI Agents
- Real Estate
- Commercial Real Estate
- Infrastructure
- Construction
- ESG
- Due Diligence
---
