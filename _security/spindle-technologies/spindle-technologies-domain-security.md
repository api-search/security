---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: spindle.ai
  spf: true
hosts:
- cert_expires: Oct 18 12:37:57 2026 GMT
  host: spindle.ai
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spindle Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spindle Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Spindle Technologies
provider_slug: spindle-technologies
slug: spindle-technologies-domain-security
source_filename: spindle-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spindle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:37:57 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: spindle.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spindle-technologies/refs/heads/main/security/spindle-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Agents
- Salesforce
- Acquired
---
