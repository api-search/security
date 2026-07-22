---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lean.org
  spf: true
hosts:
- cert_expires: Sep 23 13:03:38 2026 GMT
  host: www.lean.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lean Six Sigma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lean Six Sigma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lean Six Sigma
provider_slug: lean-six-sigma
slug: lean-six-sigma-domain-security
source_filename: lean-six-sigma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lean.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:03:38 2026 GMT\n  hsts: false\ndomains:\n- domain: lean.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-six-sigma/refs/heads/main/security/lean-six-sigma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Process
- Continuous Improvement
- Methodology
- Process Improvement
- Quality Management
---
