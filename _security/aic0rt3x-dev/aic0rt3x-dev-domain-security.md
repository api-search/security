---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aic0rt3x.dev
  spf: true
hosts:
- cert_expires: Jan  1 05:46:28 2027 GMT
  host: aic0rt3x.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aic0Rt3X Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Cortex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AI Cortex
provider_slug: aic0rt3x-dev
slug: aic0rt3x-dev-domain-security
source_filename: aic0rt3x-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aic0rt3x.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:46:28 2027 GMT\n  hsts: false\ndomains:\n- domain: aic0rt3x.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aic0rt3x-dev/security/aic0rt3x-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Infrastructure
- Agents
- Cloud
- Platform
---
