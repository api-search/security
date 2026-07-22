---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: defakto.security
  spf: true
hosts:
- cert_expires: Sep  3 22:28:46 2026 GMT
  host: www.defakto.security
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spirl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spirl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Spirl
provider_slug: spirl
slug: spirl-domain-security
source_filename: spirl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.defakto.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:28:46 2026 GMT\n  hsts: false\ndomains:\n- domain: defakto.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spirl/refs/heads/main/security/spirl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Identity
- Non-Human Identity
- Workload Identity
- SPIFFE
- Secrets Management
- Zero Trust
- CI/CD Security
- Kubernetes
- AI Agents
---
