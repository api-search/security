---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fabrix.security
  spf: true
hosts:
- cert_expires: Oct  5 23:41:28 2026 GMT
  host: fabrix.security
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fabrix
provider_slug: fabrix
slug: fabrix-domain-security
source_filename: fabrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabrix.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:41:28 2026 GMT\n  hsts: false\ndomains:\n- domain: fabrix.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabrix/refs/heads/main/security/fabrix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Identity
- Identity and Access Management
- IAM
- Security
- Cybersecurity
- AI Agents
- Access Governance
- Non-Human Identity
---
