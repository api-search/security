---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tunetx.com
  spf: true
hosts:
- cert_expires: Oct 16 00:30:50 2026 GMT
  host: tunetx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tune Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tune Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tune Therapeutics
provider_slug: tune-therapeutics
slug: tune-therapeutics-domain-security
source_filename: tune-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tunetx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tunetx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tune-therapeutics/refs/heads/main/security/tune-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Genomics
- Epigenetics
- Gene Therapy
- Clinical Stage
- Research
---
