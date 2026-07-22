---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deepgenomics.com
  spf: true
hosts:
- cert_expires: Oct 15 10:07:00 2026 GMT
  host: www.deepgenomics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Deep Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deep Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deep Genomics
provider_slug: deep-genomics
slug: deep-genomics-domain-security
source_filename: deep-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deepgenomics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 10:07:00 2026 GMT\n  hsts: false\ndomains:\n- domain: deepgenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deep-genomics/refs/heads/main/security/deep-genomics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- Genomics
- Biotechnology
- Drug Discovery
- Genetic Medicine
- Healthcare
- Machine Learning
---
