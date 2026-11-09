---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bancada.es
  spf: true
hosts:
- cert_expires: Dec 20 10:57:21 2026 GMT
  host: bancada.es
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bancada Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bancada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bancada
provider_slug: bancada-es
slug: bancada-es-domain-security
source_filename: bancada-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bancada.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:57:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bancada.es\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bancada-es/security/bancada-es-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- IoT
- Hardware
- Software
- Engineering
---
