---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: qxotic.ai
  spf: true
hosts:
- cert_expires: Dec 28 12:00:49 2026 GMT
  host: qxotic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qxotic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quixotic AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Quixotic AI
provider_slug: qxotic
slug: qxotic-domain-security
source_filename: qxotic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qxotic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 12:00:49 2026 GMT\n  hsts: false\ndomains:\n- domain: qxotic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/qxotic/security/qxotic-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- JVM
- Open Source
- Modular
---
