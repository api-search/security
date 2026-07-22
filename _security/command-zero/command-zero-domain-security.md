---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cmdzero.io
  spf: true
hosts:
- cert_expires: Oct 12 21:11:52 2026 GMT
  host: www.cmdzero.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Command Zero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Command Zero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Command Zero
provider_slug: command-zero
slug: command-zero-domain-security
source_filename: command-zero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cmdzero.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:11:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cmdzero.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/command-zero/refs/heads/main/security/command-zero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- SOC
- Investigations
- Threat Detection
- Incident Response
- Artificial Intelligence
- Agents
- Governed AI
---
