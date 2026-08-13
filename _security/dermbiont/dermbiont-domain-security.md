---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dermbiont.com
  spf: true
hosts:
- cert_expires: Oct 16 23:33:57 2026 GMT
  host: www.dermbiont.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dermbiont Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DermBiont, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DermBiont
provider_slug: dermbiont
slug: dermbiont-domain-security
source_filename: dermbiont-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dermbiont.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:33:57 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: dermbiont.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dermbiont/refs/heads/main/security/dermbiont-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Dermatology
- Therapeutics
- Skin Microbiome
- Microbiome
- Drug Discovery
- Clinical Stage
- Life Sciences
- Health
---
