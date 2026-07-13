---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pytorch.org
  spf: true
hosts:
- cert_expires: Sep 28 11:44:15 2026 GMT
  host: pytorch.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pytorch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PyTorch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PyTorch
provider_slug: pytorch
slug: pytorch-domain-security
source_filename: pytorch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pytorch.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:44:15 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: pytorch.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pytorch/refs/heads/main/security/pytorch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Deep Learning
- Machine Learning
- Neural Networks
- Open Source
- Python
---
