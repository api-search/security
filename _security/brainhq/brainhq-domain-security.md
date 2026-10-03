---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brainhq.com
  spf: true
hosts:
- cert_expires: Nov 27 23:49:26 2026 GMT
  host: www.brainhq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainhq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrainHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrainHQ
provider_slug: brainhq
slug: brainhq-domain-security
source_filename: brainhq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brainhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:49:26 2026 GMT\n  hsts: false\ndomains:\n- domain: brainhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainhq/refs/heads/main/security/brainhq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Brain-Training
- Cognitive-Health
- SaaS
- Posit-Science
---
