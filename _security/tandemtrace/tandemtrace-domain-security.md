---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tandemtrace.ai
  spf: true
hosts:
- cert_expires: Jan 14 17:45:42 2027 GMT
  host: tandemtrace.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tandemtrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TandemTrace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TandemTrace
provider_slug: tandemtrace
slug: tandemtrace-domain-security
source_filename: tandemtrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tandemtrace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 17:45:42 2027 GMT\n  hsts: false\ndomains:\n- domain: tandemtrace.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tandemtrace/security/tandemtrace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- AI
- SOC
- Automation
---
