---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dovellabs.si
  spf: true
hosts:
- cert_expires: Jan  7 03:02:45 2027 GMT
  host: dovellabs.si
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dovel Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dovel Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dovel Labs
provider_slug: dovellabs-si
slug: dovellabs-si-domain-security
source_filename: dovellabs-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dovellabs.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 03:02:45 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dovellabs.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dovellabs-si/security/dovellabs-si-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- API Change Monitoring
- SDK Migration
- AI Agents
- Agent Observability
- Pull Request Automation
---
