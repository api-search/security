---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: litmus.io
  spf: true
hosts:
- cert_expires: Sep 16 20:01:18 2026 GMT
  host: litmus.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 09:48:32 2026 GMT
  host: api.litmus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Litmus Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Litmus Automation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Litmus Automation
provider_slug: litmus-automation
slug: litmus-automation-domain-security
source_filename: litmus-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: litmus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:01:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.litmus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 09:48:32 2026 GMT\n  hsts: false\ndomains:\n- domain: litmus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litmus-automation/refs/heads/main/security/litmus-automation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- Industrial IoT
- Edge Computing
- IIoT
- Unified Namespace
- MQTT
- DataOps
- Industrial Data Platform
- Analytics
---
