---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neostella.com
  spf: true
hosts:
- cert_expires: Dec 23 20:41:34 2026 GMT
  host: neostella.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Neostella Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neostella, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neostella
provider_slug: neostella
slug: neostella-domain-security
source_filename: neostella-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neostella.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:41:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: neostella.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/neostella/security/neostella-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LegalTech
- SaaS
- CaseManagement
- Enterprise
---
