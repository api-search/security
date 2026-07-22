---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: walter.one
  spf: false
hosts:
- cert_expires: Oct 19 14:52:11 2026 GMT
  host: www.walter.one
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Walter
provider_slug: walter
slug: walter-domain-security
source_filename: walter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walter.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 14:52:11 2026 GMT\n  hsts: false\ndomains:\n- domain: walter.one\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walter/refs/heads/main/security/walter-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agent
- Manufacturing
- ERP
- Automation
- Document Processing
- Procurement
- Y Combinator
---
