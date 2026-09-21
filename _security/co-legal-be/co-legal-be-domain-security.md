---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: co-legal.be
  spf: true
hosts:
- cert_expires: Oct 24 12:29:50 2026 GMT
  host: co-legal.be
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 14:24:28 2026 GMT
  host: agent.co-legal.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Co Legal Be Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Co-Legal B.V., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Co-Legal B.V.
provider_slug: co-legal-be
slug: co-legal-be-domain-security
source_filename: co-legal-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: co-legal.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 12:29:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: agent.co-legal.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 14:24:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: co-legal.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-legal-be/refs/heads/main/security/co-legal-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Legal Research
- Tax
- Case Law
- Legislation
- Company Registry
- VAT Validation
- Belgium
- Netherlands
- European Union
- A2A
- MCP
- agent-native
- Artificial Intelligence
- Legal Tech
---
