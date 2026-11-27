---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: corply.dev
  spf: true
hosts:
- cert_expires: Jan  1 05:12:49 2027 GMT
  host: corply.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Corply
provider_slug: corply-dev
slug: corply-dev-domain-security
source_filename: corply-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corply.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:12:49 2027 GMT\n  hsts: false\ndomains:\n- domain: corply.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/corply-dev/security/corply-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Company Formation
- Incorporation
- Delaware C-Corp
- Legal Tech
- AI Agents
- MCP
- Startups
---
