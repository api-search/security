---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pharmazz.com
  spf: true
hosts:
- cert_expires: Sep  4 14:39:07 2026 GMT
  host: www.pharmazz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pharmazz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pharmazz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pharmazz
provider_slug: pharmazz
slug: pharmazz-domain-security
source_filename: pharmazz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pharmazz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:39:07 2026 GMT\n  hsts: false\ndomains:\n- domain: pharmazz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pharmazz/refs/heads/main/security/pharmazz-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Life Sciences
- Healthcare
- Clinical Trials
- Critical Care
- Drug Development
---
