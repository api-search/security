---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: achira.ai
  spf: true
hosts:
- cert_expires: Sep 10 09:48:49 2026 GMT
  host: achira.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Achira Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Achira, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Achira
provider_slug: achira
slug: achira-domain-security
source_filename: achira-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: achira.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:48:49 2026 GMT\n  hsts: false\ndomains:\n- domain: achira.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/achira/refs/heads/main/security/achira-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Biology
- Drug Discovery
- Molecular Simulation
- Machine Learning
- Quantum Chemistry
- Computational Chemistry
- Artificial Intelligence
- Life Sciences
---
