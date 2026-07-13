---
api_specs:
- filename: tsinghua-tuna-mirror-status.yaml
  format: yaml
  label: TUNA Mirror Sync Status API
  slug: tuna-mirror-status
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/openapi/tsinghua-tuna-mirror-status.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tsinghua.edu.cn
  spf: true
hosts:
- cert_expires: Sep 11 15:05:35 2026 GMT
  host: www.tsinghua.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 13 14:15:41 2026 GMT
  host: mirrors.tuna.tsinghua.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsinghua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tsinghua University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tsinghua University
provider_slug: tsinghua
slug: tsinghua-domain-security
source_filename: tsinghua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsinghua.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:05:35 2026 GMT\n  hsts: false\n- host: mirrors.tuna.tsinghua.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 13 14:15:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tsinghua.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/security/tsinghua-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- China
- Open Source
---
