---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1qbit.com
  spf: true
hosts:
- cert_expires: Sep 30 23:02:10 2026 GMT
  host: 1qbit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Qbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1QBit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 1QBit
provider_slug: 1qbit
slug: 1qbit-domain-security
source_filename: 1qbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1qbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:02:10 2026 GMT\n  hsts: false\ndomains:\n- domain: 1qbit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1qbit/refs/heads/main/security/1qbit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Quantum Computing
- Optimization
- Machine Learning
- Simulation
- Scientific Computing
- Research
- Canada
---
