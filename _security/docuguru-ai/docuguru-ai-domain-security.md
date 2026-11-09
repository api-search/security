---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docuguru.ai
  spf: true
hosts:
- cert_expires: Jan  1 00:11:15 2027 GMT
  host: docuguru.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docuguru Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocuGuru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DocuGuru
provider_slug: docuguru-ai
slug: docuguru-ai-domain-security
source_filename: docuguru-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docuguru.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 00:11:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: docuguru.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/docuguru-ai/security/docuguru-ai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
---
