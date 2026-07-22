---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: lattice-engines.com
  spf: true
hosts:
- cert_expires: Oct  7 13:43:22 2026 GMT
  host: www.lattice-engines.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lattice Engines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lattice Engines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Lattice Engines
provider_slug: lattice-engines
slug: lattice-engines-domain-security
source_filename: lattice-engines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lattice-engines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:43:22 2026 GMT\n  hsts: null\ndomains:\n- domain: lattice-engines.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattice-engines/refs/heads/main/security/lattice-engines-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Acquired
- Predictive Marketing
- Account Based Marketing
- Sales Intelligence
- Customer Data Platform
- Lead Scoring
- Machine Learning
- B2B Marketing
- Historical
---
