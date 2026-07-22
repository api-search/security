---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cognitivespace.com
  spf: true
hosts:
- cert_expires: Sep  7 06:55:04 2026 GMT
  host: cognitivespace.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognitive Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognitive Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cognitive Space
provider_slug: cognitive-space
slug: cognitive-space-domain-security
source_filename: cognitive-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognitivespace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:55:04 2026 GMT\n  hsts: false\ndomains:\n- domain: cognitivespace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognitive-space/refs/heads/main/security/cognitive-space-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aerospace
- Satellite
- Space
- Artificial Intelligence
- Satellite Operations
- Constellation Management
- Data as a Service
- Government
- Defense
---
