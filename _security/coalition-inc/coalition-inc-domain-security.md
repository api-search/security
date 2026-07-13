---
api_specs:
- filename: openapi.json
  format: json
  label: Coalition Exploit Scoring System (ESS) API
  slug: exploit-scoring-system
  spec_type: OpenAPI
  url: https://ess-api.coalitioninc.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coalitioninc.com
  spf: true
hosts:
- cert_expires: Oct  9 10:54:39 2026 GMT
  host: www.coalitioninc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:42:44 2026 GMT
  host: ess.coalitioninc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:42:44 2026 GMT
  host: ess-api.coalitioninc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coalition Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coalition, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coalition
provider_slug: coalition-inc
slug: coalition-inc-domain-security
source_filename: coalition-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coalitioninc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 10:54:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ess.coalitioninc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:42:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ess-api.coalitioninc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:42:44 2026 GMT\n  hsts: null\ndomains:\n- domain: coalitioninc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalition-inc/refs/heads/main/security/coalition-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cyber Insurance
- Insurance
- Insurtech
- Risk Management
- Cybersecurity
- Vulnerability Management
- CVE
- Exploit Scoring
- Threat Intelligence
- Incident Response
- Attack Surface Management
- Brokers
- MGA
- Executive Risks
- Technology E&O
- Active Insurance
---
