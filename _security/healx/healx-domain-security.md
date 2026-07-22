---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: healx.ai
  spf: true
hosts:
- cert_expires: Aug 22 11:47:22 2026 GMT
  host: healx.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Healx
provider_slug: healx
slug: healx-domain-security
source_filename: healx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:47:22 2026 GMT\n  hsts: false\ndomains:\n- domain: healx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healx/refs/heads/main/security/healx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Drug Discovery
- Rare Diseases
- Biotechnology
- Healthcare
- Life Sciences
- Machine Learning
---
