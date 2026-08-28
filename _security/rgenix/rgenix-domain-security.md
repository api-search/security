---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: inspirna.com
  spf: true
hosts:
- cert_expires: Sep 27 02:45:15 2026 GMT
  host: inspirna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rgenix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rgenix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Rgenix
provider_slug: rgenix
slug: rgenix-domain-security
source_filename: rgenix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inspirna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:45:15 2026 GMT\n  hsts: false\ndomains:\n- domain: inspirna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rgenix/refs/heads/main/security/rgenix-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Drug Discovery
- Clinical Trials
- Life Sciences
---
