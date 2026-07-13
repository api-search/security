---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deepai.org
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: deepai.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DeepAI
provider_slug: deepai
slug: deepai-domain-security
source_filename: deepai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepai.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: deepai.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepai/refs/heads/main/security/deepai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Machine Learning
- Public APIs
---
