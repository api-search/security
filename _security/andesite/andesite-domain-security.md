---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: andesite.ai
  spf: true
hosts:
- cert_expires: Oct 11 15:54:16 2026 GMT
  host: andesite.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Andesite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andesite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Andesite
provider_slug: andesite
slug: andesite-domain-security
source_filename: andesite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andesite.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 15:54:16 2026 GMT\n  hsts: false\ndomains:\n- domain: andesite.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andesite/refs/heads/main/security/andesite-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Defense Government
- Cybersecurity
- Security Operations
- Artificial Intelligence
- Threat Detection
- SOC
- Compliance
---
