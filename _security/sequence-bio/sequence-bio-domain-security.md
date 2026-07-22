---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sequencebio.com
  spf: true
hosts:
- cert_expires: Sep 27 00:50:55 2026 GMT
  host: www.sequencebio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequence Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequence Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sequence Bio
provider_slug: sequence-bio
slug: sequence-bio-domain-security
source_filename: sequence-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sequencebio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:50:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sequencebio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequence-bio/refs/heads/main/security/sequence-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Genomics
- Life Sciences
- Biotechnology
- Population Genetics
- Drug Discovery
- Healthcare
- Research
---
