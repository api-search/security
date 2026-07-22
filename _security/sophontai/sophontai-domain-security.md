---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sophont.med
  spf: true
hosts:
- cert_expires: Oct  3 16:49:06 2026 GMT
  host: sophont.med
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sophontai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sophont, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sophont
provider_slug: sophontai
slug: sophontai-domain-security
source_filename: sophontai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sophont.med\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:49:06 2026 GMT\n  hsts: false\ndomains:\n- domain: sophont.med\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sophontai/refs/heads/main/security/sophontai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Healthcare
- Medical Imaging
- Foundation Models
- Open Source
- Research
---
