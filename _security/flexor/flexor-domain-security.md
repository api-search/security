---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flexor.ai
  spf: true
hosts:
- cert_expires: Nov 23 21:06:17 2026 GMT
  host: flexor.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flexor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flexor
provider_slug: flexor
slug: flexor-domain-security
source_filename: flexor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexor.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 21:06:17 2026 GMT\n  hsts: false\ndomains:\n- domain: flexor.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flexor/security/flexor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Data Platform
- Enterprise
- Unstructured Data
---
