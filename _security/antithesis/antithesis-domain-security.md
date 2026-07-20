---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: antithesis.com
  spf: true
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: antithesis.com
  hsts: true
  hsts_max_age: 2678400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antithesis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antithesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Antithesis
provider_slug: antithesis
slug: antithesis-domain-security
source_filename: antithesis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antithesis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2678400\ndomains:\n- domain: antithesis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antithesis/refs/heads/main/security/antithesis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Testing
- Software Testing
- Deterministic Simulation
- Fuzzing
- Reliability
- Distributed Systems
- SDK
---
