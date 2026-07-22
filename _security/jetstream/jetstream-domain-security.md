---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jetstream.security
  spf: true
hosts:
- cert_expires: Sep 24 02:31:36 2026 GMT
  host: jetstream.security
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetstream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jetstream
provider_slug: jetstream
slug: jetstream-domain-security
source_filename: jetstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jetstream.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:31:36 2026 GMT\n  hsts: false\ndomains:\n- domain: jetstream.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetstream/refs/heads/main/security/jetstream-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cybersecurity
- AI Governance
- AI Security
- Agentic AI
- Runtime Governance
- Compliance
- FinOps
---
