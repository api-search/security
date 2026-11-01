---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: replicas.dev
  spf: true
hosts:
- cert_expires: Jan 19 15:57:37 2027 GMT
  host: replicas.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Replicas Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replicas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Replicas
provider_slug: replicas-dev
slug: replicas-dev-domain-security
source_filename: replicas-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: replicas.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:57:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: replicas.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/replicas-dev/security/replicas-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Cloud
- Platform
- Development
---
