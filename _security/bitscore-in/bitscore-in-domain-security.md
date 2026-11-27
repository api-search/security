---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:security@bitscore.in"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bitscore.in
  spf: true
hosts:
- cert_expires: Dec  3 20:22:16 2026 GMT
  host: bitscore.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BitScore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitScore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BitScore
provider_slug: bitscore-in
slug: bitscore-in-domain-security
source_filename: bitscore-in-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitscore.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 20:22:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitscore.in\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:security@bitscore.in\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bitscore-in/security/bitscore-in-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Risk Management
- Ratings
- Enterprise
- India
---
