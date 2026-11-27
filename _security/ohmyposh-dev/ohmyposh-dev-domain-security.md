---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ohmyposh.dev
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: ohmyposh.dev
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Oh My Posh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oh My Posh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Oh My Posh
provider_slug: ohmyposh-dev
slug: ohmyposh-dev-domain-security
source_filename: ohmyposh-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ohmyposh.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: ohmyposh.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ohmyposh-dev/security/ohmyposh-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Prompt Engine
- Open Source
- Go
- Cross-Platform
- Shell
---
