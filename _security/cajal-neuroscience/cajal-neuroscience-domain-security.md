---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cajal-tx.com
  spf: true
hosts:
- cert_expires: Oct 17 06:13:57 2026 GMT
  host: www.cajal-tx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cajal Neuroscience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cajal Neuroscience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cajal Neuroscience
provider_slug: cajal-neuroscience
slug: cajal-neuroscience-domain-security
source_filename: cajal-neuroscience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cajal-tx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 06:13:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cajal-tx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cajal-neuroscience/refs/heads/main/security/cajal-neuroscience-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Neurodegeneration
- Neuroscience
- Therapeutics
- Life Sciences
- Genomics
- Health
---
