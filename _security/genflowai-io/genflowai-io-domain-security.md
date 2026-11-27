---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genflowai.io
  spf: true
hosts:
- cert_expires: Jan 16 09:00:18 2027 GMT
  host: genflowai.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GenflowAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenflowAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GenflowAI
provider_slug: genflowai-io
slug: genflowai-io-domain-security
source_filename: genflowai-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genflowai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 09:00:18 2027 GMT\n  hsts: false\ndomains:\n- domain: genflowai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/genflowai-io/security/genflowai-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Content
- Templates
- Commerce
---
