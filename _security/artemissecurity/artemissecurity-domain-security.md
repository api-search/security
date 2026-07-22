---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: artemissecurity.com
  spf: true
hosts:
- cert_expires: Sep  3 10:48:08 2026 GMT
  host: artemissecurity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Artemissecurity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artemis Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Artemis Security
provider_slug: artemissecurity
slug: artemissecurity-domain-security
source_filename: artemissecurity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artemissecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 10:48:08 2026 GMT\n  hsts: false\ndomains:\n- domain: artemissecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artemissecurity/refs/heads/main/security/artemissecurity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Cybersecurity
- Threat Detection
- Security Operations
- SIEM
- AI
- SOC
- Cloud Security
---
