---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: latticeflow.ai
  spf: true
hosts:
- cert_expires: Dec  5 15:09:25 2026 GMT
  host: latticeflow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latticeflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LatticeFlow AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LatticeFlow AI
provider_slug: latticeflow
slug: latticeflow-domain-security
source_filename: latticeflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latticeflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 15:09:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: latticeflow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/latticeflow/security/latticeflow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Governance
- RiskManagement
- Enterprise
---
