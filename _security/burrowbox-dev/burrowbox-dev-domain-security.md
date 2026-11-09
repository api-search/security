---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: burrowbox.dev
  spf: true
hosts:
- cert_expires: Dec 29 19:04:08 2026 GMT
  host: burrowbox.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Burrowbox Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Burrowbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Burrowbox
provider_slug: burrowbox-dev
slug: burrowbox-dev-domain-security
source_filename: burrowbox-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: burrowbox.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 19:04:08 2026 GMT\n  hsts: false\ndomains:\n- domain: burrowbox.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/burrowbox-dev/security/burrowbox-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Agents
- Linux Desktop
- Persistent Browser
- Credential Vault
- Pay‑per‑minute
- SaaS Platform
---
