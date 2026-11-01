---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pallie.ai
  spf: false
hosts:
- cert_expires: Dec 12 17:30:06 2026 GMT
  host: pallie.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pallie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pallie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Pallie
provider_slug: pallie
slug: pallie-domain-security
source_filename: pallie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pallie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:30:06 2026 GMT\n  hsts: false\ndomains:\n- domain: pallie.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pallie/security/pallie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Personal Companion
- Mental Health
- Productivity
---
