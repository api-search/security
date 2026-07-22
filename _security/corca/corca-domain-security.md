---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: corca.io
  spf: true
hosts:
- cert_expires: Sep  3 19:32:32 2026 GMT
  host: corca.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Corca
provider_slug: corca
slug: corca-domain-security
source_filename: corca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corca.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:32:32 2026 GMT\n  hsts: false\ndomains:\n- domain: corca.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corca/refs/heads/main/security/corca-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Mathematics
- Collaboration
- Productivity
- LaTeX
- Editor
- Artificial Intelligence
- Research
- Education
---
