---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jam.dev
  spf: true
hosts:
- cert_expires: Oct  6 00:54:02 2026 GMT
  host: jam.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jam
provider_slug: jam
slug: jam-domain-security
source_filename: jam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jam.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:54:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jam.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jam/refs/heads/main/security/jam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Bug Reporting
- Debugging
- Quality Assurance
- Observability
- Screen Recording
- Model Context Protocol
---
