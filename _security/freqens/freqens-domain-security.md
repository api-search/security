---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freqens.com
  spf: true
hosts:
- cert_expires: Sep 10 11:14:38 2026 GMT
  host: freqens.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freqens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freqens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freqens
provider_slug: freqens
slug: freqens-domain-security
source_filename: freqens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freqens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:14:38 2026 GMT\n  hsts: false\ndomains:\n- domain: freqens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freqens/refs/heads/main/security/freqens-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Planning and Analysis
- FP&A
- Finance
- CFO
- Fintech
- Agentic AI
- SaaS
---
