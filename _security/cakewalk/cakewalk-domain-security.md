---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cakewalk.security
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getcakewalk.io
  spf: true
hosts:
- cert_expires: Aug 24 06:54:50 2026 GMT
  host: www.cakewalk.security
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 00:50:56 2026 GMT
  host: open-api.getcakewalk.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cakewalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cakewalk, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cakewalk
provider_slug: cakewalk
slug: cakewalk-domain-security
source_filename: cakewalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cakewalk.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:54:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: open-api.getcakewalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 00:50:56 2026 GMT\n  hsts: null\ndomains:\n- domain: cakewalk.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getcakewalk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cakewalk/refs/heads/main/security/cakewalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Access Management
- Identity Governance
- IGA
- AI Agents
- Security
- Access Control
- MCP
- Provisioning
- SaaS Management
- Authentication
---
