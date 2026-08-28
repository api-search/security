---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medeortx.com
  spf: true
hosts:
- cert_expires: Jan 18 10:46:52 2027 GMT
  host: medeortx.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Medeor Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medeor Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Medeor Therapeutics
provider_slug: medeor-therapeutics
slug: medeor-therapeutics-domain-security
source_filename: medeor-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medeortx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 18 10:46:52 2027 GMT\n  hsts: false\ndomains:\n- domain: medeortx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medeor-therapeutics/refs/heads/main/security/medeor-therapeutics-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotechnology
- Life Sciences
- Cell Therapy
- Immunotherapy
- Organ Transplant
- Healthcare
- Clinical Trials
- Pharmaceuticals
---
