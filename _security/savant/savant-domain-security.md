---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heysavant.com
  spf: false
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: heysavant.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Savant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Savant
provider_slug: savant
slug: savant-domain-security
source_filename: savant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heysavant.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: heysavant.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savant/refs/heads/main/security/savant-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Knowledge Management
- Artificial Intelligence
- AI Agents
- Enterprise Knowledge
- Operational Memory
- Y Combinator
---
