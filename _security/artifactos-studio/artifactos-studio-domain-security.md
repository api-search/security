---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: artifactos.studio
  spf: false
hosts:
- cert_expires: Jan 28 06:26:08 2027 GMT
  host: artifactos.studio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artifactos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artifactos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Artifactos
provider_slug: artifactos-studio
slug: artifactos-studio-domain-security
source_filename: artifactos-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: artifactos.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 06:26:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: artifactos.studio\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/artifactos-studio/security/artifactos-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Insurance
- Artificial Intelligence
- Automation
- WhatsApp
- Latin America
---
