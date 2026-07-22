---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fabletherapeutics.com
  spf: true
hosts:
- cert_expires: Sep 29 19:02:52 2026 GMT
  host: fabletherapeutics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fable Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fable Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fable Therapeutics
provider_slug: fable-therapeutics
slug: fable-therapeutics-domain-security
source_filename: fable-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabletherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:02:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fabletherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fable-therapeutics/refs/heads/main/security/fable-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Therapeutics
- Obesity
- Metabolic Disease
- Drug Discovery
- Protein Engineering
- Biologics
---
