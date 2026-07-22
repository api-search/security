---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: crafting.dev
  spf: true
hosts:
- cert_expires: Aug 25 12:52:03 2026 GMT
  host: crafting.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crafting Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crafting, Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Crafting, Inc.
provider_slug: crafting-inc
slug: crafting-inc-domain-security
source_filename: crafting-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crafting.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:52:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crafting.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crafting-inc/refs/heads/main/security/crafting-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- AI Sandboxes
- Coding Agents
- Developer Environments
- CI/CD
- Kubernetes
- Developer Productivity
- Infrastructure
---
