---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartdiagnosticssystems.com
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: smartdiagnosticssystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smart Diagnostics Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smart Diagnostics Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Smart Diagnostics Systems
provider_slug: smart-diagnostics-systems
slug: smart-diagnostics-systems-domain-security
source_filename: smart-diagnostics-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartdiagnosticssystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: smartdiagnosticssystems.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smart-diagnostics-systems/refs/heads/main/security/smart-diagnostics-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food Safety
- Diagnostics
- Pathogen Detection
- Biotechnology
- Health Technology
---
