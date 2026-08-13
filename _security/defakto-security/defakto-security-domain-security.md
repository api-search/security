---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: defakto.security
  spf: true
hosts:
- cert_expires: Nov  1 22:21:02 2026 GMT
  host: www.defakto.security
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 12:41:16 2026 GMT
  host: d.defakto.security
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: api.defakto.security
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Defakto Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Defakto Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Defakto Security
provider_slug: defakto-security
slug: defakto-security-domain-security
source_filename: defakto-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defakto.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 22:21:02 2026 GMT\n  hsts: false\n- host: d.defakto.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 12:41:16 2026 GMT\n  hsts: false\n- host: api.defakto.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: defakto.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/defakto-security/refs/heads/main/security/defakto-security-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Security
- Identity
- Non-Human Identity
- Workload Identity
- SPIFFE
- Authentication
- Zero Trust
- Secrets Management
- Kubernetes
- CI/CD
- Cloud Security
- gRPC
- Machine Identity
- Agentic AI
---
