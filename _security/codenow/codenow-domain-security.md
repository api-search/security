---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codenow.com
  spf: true
hosts:
- cert_expires: Sep 28 04:30:52 2026 GMT
  host: docs.codenow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.codenow.com
  https: false
kind: domain-security
layout: security
method: probed
name: Codenow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeNOW, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CodeNOW
provider_slug: codenow
slug: codenow-domain-security
source_filename: codenow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.codenow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 04:30:52 2026 GMT\n  hsts: false\n- host: api.codenow.com\n  https: false\ndomains:\n- domain: codenow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codenow/refs/heads/main/security/codenow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- DevOps
- Software Delivery
- Platform Engineering
- Governance
- AI Agents
- CI/CD
- Deployment
- Kubernetes
- Model Context Protocol
---
