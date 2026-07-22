---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solutherapeutics.com
  spf: true
hosts:
- cert_expires: Oct  8 01:29:53 2026 GMT
  host: solutherapeutics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solu Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solu Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solu Therapeutics
provider_slug: solu-therapeutics
slug: solu-therapeutics-domain-security
source_filename: solu-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solutherapeutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: solutherapeutics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solu-therapeutics/refs/heads/main/security/solu-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Therapeutics
- Oncology
- Immunology
- Antibodies
- Drug Discovery
- Clinical Stage
---
