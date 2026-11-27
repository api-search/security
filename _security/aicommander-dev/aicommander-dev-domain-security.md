---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aicommander.dev
  spf: true
hosts:
- cert_expires: Jan 22 21:25:16 2027 GMT
  host: aicommander.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Commander Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Commander, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AI Commander
provider_slug: aicommander-dev
slug: aicommander-dev-domain-security
source_filename: aicommander-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aicommander.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 21:25:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aicommander.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aicommander-dev/security/aicommander-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- RemoteShell
- Machine Learning
- Automation
- Cloud
---
