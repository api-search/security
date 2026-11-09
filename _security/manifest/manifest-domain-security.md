---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: manifest.build
  spf: true
hosts:
- cert_expires: Jan 29 16:31:09 2027 GMT
  host: manifest.build
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Manifest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manifest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Manifest
provider_slug: manifest
slug: manifest-domain-security
source_filename: manifest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manifest.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 16:31:09 2027 GMT\n  hsts: false\ndomains:\n- domain: manifest.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/manifest/security/manifest-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LLM Gateway
- AI Agents
- Artificial Intelligence
- Open Source
- Observability
- OpenAI-Compatible
- Self-Hosted
---
