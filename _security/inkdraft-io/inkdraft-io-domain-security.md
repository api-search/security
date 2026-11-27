---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: inkdraft.io
  spf: true
hosts:
- cert_expires: Jan  5 23:56:21 2027 GMT
  host: inkdraft.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InkDraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InkDraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: InkDraft
provider_slug: inkdraft-io
slug: inkdraft-io-domain-security
source_filename: inkdraft-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inkdraft.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:56:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inkdraft.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/inkdraft-io/security/inkdraft-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software-as-a-Service
- Sales
- Artificial Intelligence
- Contracts
- Proposals
- Service Business
---
