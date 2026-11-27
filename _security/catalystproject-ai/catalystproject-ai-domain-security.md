---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: catalystproject.ai
  spf: true
hosts:
- cert_expires: Dec  5 11:27:40 2026 GMT
  host: catalystproject.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Catalyst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Catalyst, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Catalyst
provider_slug: catalystproject-ai
slug: catalystproject-ai-domain-security
source_filename: catalystproject-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalystproject.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 11:27:40 2026 GMT\n  hsts: null\ndomains:\n- domain: catalystproject.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/catalystproject-ai/security/catalystproject-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Computational Biology
- Data Platform
- Graph API
- Human Biology
- Research Tools
---
