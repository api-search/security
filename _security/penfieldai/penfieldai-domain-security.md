---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: penfield.ai
  spf: true
hosts:
- cert_expires: Oct  4 10:22:39 2026 GMT
  host: penfield.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Penfieldai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penfield.AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Penfield.AI
provider_slug: penfieldai
slug: penfieldai-domain-security
source_filename: penfieldai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: penfield.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 10:22:39 2026 GMT\n  hsts: false\ndomains:\n- domain: penfield.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penfieldai/refs/heads/main/security/penfieldai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Cybersecurity
- Security Operations
- SOC
- AI Governance
- Compliance
- Process Verification
- MSSP
- Identity and Access Management
---
