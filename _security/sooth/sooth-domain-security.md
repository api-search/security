---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soothlabs.com
  spf: false
hosts:
- cert_expires: Oct 12 12:43:46 2026 GMT
  host: soothlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sooth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sooth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Sooth
provider_slug: sooth
slug: sooth-domain-security
source_filename: sooth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soothlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 12:43:46 2026 GMT\n  hsts: false\ndomains:\n- domain: soothlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sooth/refs/heads/main/security/sooth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Forecasting
- World Model
- Foresight
- Decision Intelligence
- Risk
- Machine Learning
---
