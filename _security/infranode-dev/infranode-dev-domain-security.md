---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: infranode.dev
  spf: true
hosts:
- cert_expires: Jan  6 09:20:30 2027 GMT
  host: infranode.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Infranode Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for infranode-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: infranode-dev
provider_slug: infranode-dev
slug: infranode-dev-domain-security
source_filename: infranode-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infranode.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 09:20:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infranode.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/infranode-dev/security/infranode-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
