---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iggenix.com
  spf: false
hosts:
- cert_expires: Nov 17 16:28:16 2026 GMT
  host: iggenix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Iggenix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IgGenix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: IgGenix
provider_slug: iggenix
slug: iggenix-domain-security
source_filename: iggenix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iggenix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 16:28:16 2026 GMT\n  hsts: false\ndomains:\n- domain: iggenix.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iggenix/refs/heads/main/security/iggenix-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Life Sciences
- Immunology
- Allergy
- Antibodies
- Drug Discovery
- Therapeutics
- Clinical Trials
- Pharmaceuticals
- Research
---
