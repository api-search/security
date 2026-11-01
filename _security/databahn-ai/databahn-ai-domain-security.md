---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: databahn.ai
  spf: true
hosts:
- cert_expires: Dec 20 18:12:32 2026 GMT
  host: www.databahn.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Databahn Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataBahn.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataBahn.ai
provider_slug: databahn-ai
slug: databahn-ai-domain-security
source_filename: databahn-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.databahn.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 18:12:32 2026 GMT\n  hsts: null\ndomains:\n- domain: databahn.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/databahn-ai/security/databahn-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Pipeline
- Security
- Observability
- AI Agents
- Edge Telemetry
- Data Fabric
- SIEM Optimization
- Federated Search
---
