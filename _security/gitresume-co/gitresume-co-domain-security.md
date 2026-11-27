---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gitresume.co
  spf: true
hosts:
- cert_expires: Dec 12 10:23:20 2026 GMT
  host: gitresume.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GitResume Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitResume, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GitResume
provider_slug: gitresume-co
slug: gitresume-co-domain-security
source_filename: gitresume-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitresume.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 10:23:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gitresume.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gitresume-co/security/gitresume-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Resume
- YAML
- PDF
- Web
- Automation
---
