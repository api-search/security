---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: auditon.co
  spf: true
hosts:
- cert_expires: Dec 19 14:35:06 2026 GMT
  host: auditon.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Auditon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auditon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Auditon
provider_slug: auditon-co
slug: auditon-co-domain-security
source_filename: auditon-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: auditon.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 14:35:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: auditon.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/auditon-co/security/auditon-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Vulnerability Scanning
- Software-as-a-Service
- Compliance
- Small-Team
---
