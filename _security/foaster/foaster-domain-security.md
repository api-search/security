---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: foaster.ai
  spf: true
hosts:
- cert_expires: Sep  8 00:38:27 2026 GMT
  host: foaster.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Foaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foaster, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Foaster
provider_slug: foaster
slug: foaster-domain-security
source_filename: foaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foaster.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 00:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foaster.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foaster/refs/heads/main/security/foaster-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Transformation
- Consulting
- Professional Services
- Enterprise
- AI Agents
- Y Combinator
---
