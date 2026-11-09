---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dilohost.es
  spf: true
hosts:
- cert_expires: Jan  1 16:10:07 2027 GMT
  host: dilohost.es
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dilohost Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dilohost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dilohost
provider_slug: dilohost-es
slug: dilohost-es-domain-security
source_filename: dilohost-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dilohost.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 16:10:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dilohost.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dilohost-es/security/dilohost-es-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hosting
- Web Hosting
- MCP
- AI Agents
- Database
- Domains
- Email
- European Union
---
