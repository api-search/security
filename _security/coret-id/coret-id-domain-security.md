---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coret.id
  spf: true
hosts:
- cert_expires: Jan 23 12:10:08 2027 GMT
  host: coret.id
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: coret.id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for coret.id, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: coret.id
provider_slug: coret-id
slug: coret-id-domain-security
source_filename: coret-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coret.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:10:08 2027 GMT\n  hsts: false\ndomains:\n- domain: coret.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coret-id/security/coret-id-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mind Mapping
- Collaboration
- Productivity
- AI Agents
- MCP
- Indonesia
---
