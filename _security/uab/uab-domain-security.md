---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uab.cat
  spf: true
hosts:
- cert_expires: Nov 22 08:53:44 2026 GMT
  host: www.uab.cat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: ddd.uab.cat
  https: false
kind: domain-security
layout: security
method: probed
name: Uab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autonomous University of Barcelona, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autonomous University of Barcelona
provider_slug: uab
slug: uab-domain-security
source_filename: uab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uab.cat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 08:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ddd.uab.cat\n  https: false\ndomains:\n- domain: uab.cat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/security/uab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Spain
- Catalonia
- Open Access
- Institutional Repository
- OAI-PMH
- Research Data
---
