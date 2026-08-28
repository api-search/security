---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lenz-tx.com
  spf: true
hosts:
- cert_expires: Oct 30 05:04:19 2026 GMT
  host: lenz-tx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lenz Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LENZ Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LENZ Therapeutics
provider_slug: lenz-therapeutics
slug: lenz-therapeutics-domain-security
source_filename: lenz-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lenz-tx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:04:19 2026 GMT\n  hsts: false\ndomains:\n- domain: lenz-tx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lenz-therapeutics/refs/heads/main/security/lenz-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Life Sciences
- Healthcare
- Ophthalmology
- Presbyopia
- Drug Development
- Public Company
---
