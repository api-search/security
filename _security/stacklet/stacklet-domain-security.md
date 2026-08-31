---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stacklet.ai
  spf: true
hosts:
- cert_expires: Oct 29 20:57:49 2026 GMT
  host: stacklet.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stacklet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stacklet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stacklet
provider_slug: stacklet
slug: stacklet-domain-security
source_filename: stacklet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stacklet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 20:57:49 2026 GMT\n  hsts: false\ndomains:\n- domain: stacklet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacklet/refs/heads/main/security/stacklet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Governance
- Cloud Custodian
- Policy as Code
- FinOps
- Cloud Security
- Compliance
- Infrastructure as Code
- Terraform
- GraphQL
- Model Context Protocol
- Azure
- Google Cloud
- Agents
---
