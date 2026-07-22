---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 10xscience.com
  spf: true
hosts:
- cert_expires: Sep 11 01:57:58 2026 GMT
  host: 10xscience.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 10X Science Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 10x Science, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 10x Science
provider_slug: 10x-science
slug: 10x-science-domain-security
source_filename: 10x-science-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 10xscience.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:57:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 10xscience.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10x-science/refs/heads/main/security/10x-science-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Life Sciences
- Drug Discovery
- Protein Therapeutics
- Biotechnology
- Artificial Intelligence
- Peptide Mapping
---
