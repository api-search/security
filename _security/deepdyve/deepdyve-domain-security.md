---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepdyve.com
  spf: true
hosts:
- cert_expires: Dec 28 11:48:49 2026 GMT
  host: www.deepdyve.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deepdyve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepdyve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deepdyve
provider_slug: deepdyve
slug: deepdyve-domain-security
source_filename: deepdyve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepdyve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:48:49 2026 GMT\n  hsts: null\ndomains:\n- domain: deepdyve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/deepdyve/security/deepdyve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Literature
- Research
- Artificial Intelligence
- Software-as-a-Service
---
