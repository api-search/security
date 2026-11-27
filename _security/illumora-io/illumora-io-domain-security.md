---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: illumora.io
  spf: true
hosts:
- cert_expires: Dec 18 12:36:16 2026 GMT
  host: illumora.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Illumora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Illumora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Illumora
provider_slug: illumora-io
slug: illumora-io-domain-security
source_filename: illumora-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: illumora.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 12:36:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: illumora.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/illumora-io/security/illumora-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Education
- Prompt Engineering
- Literacy
- Platform
---
