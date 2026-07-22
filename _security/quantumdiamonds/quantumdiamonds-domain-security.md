---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: qd-st.com
  spf: true
hosts:
- cert_expires: Sep 13 22:11:07 2026 GMT
  host: www.qd-st.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantumdiamonds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantumdiamonds, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quantumdiamonds
provider_slug: quantumdiamonds
slug: quantumdiamonds-domain-security
source_filename: quantumdiamonds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qd-st.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:11:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qd-st.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantumdiamonds/refs/heads/main/security/quantumdiamonds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Quantum
- Quantum Sensing
- Semiconductor
- Failure Analysis
- Deep Tech
- Hardware
- Instrumentation
---
