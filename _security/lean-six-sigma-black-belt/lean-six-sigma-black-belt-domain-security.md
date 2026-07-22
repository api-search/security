---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: asq.org
  spf: true
hosts:
- cert_expires: Sep 13 18:47:35 2026 GMT
  host: www.asq.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lean Six Sigma Black Belt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lean Six Sigma Black Belt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lean Six Sigma Black Belt
provider_slug: lean-six-sigma-black-belt
slug: lean-six-sigma-black-belt-domain-security
source_filename: lean-six-sigma-black-belt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asq.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:47:35 2026 GMT\n  hsts: false\ndomains:\n- domain: asq.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-six-sigma-black-belt/refs/heads/main/security/lean-six-sigma-black-belt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lean Manufacturing
- Process Improvement
- Project Management
- Quality Management
- Six Sigma
- Statistical Analysis
---
