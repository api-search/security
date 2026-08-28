---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nextpointtx.com
  spf: true
hosts:
- cert_expires: Oct  3 01:44:16 2026 GMT
  host: nextpointtx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NextPoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NextPoint
provider_slug: nextpoint
slug: nextpoint-domain-security
source_filename: nextpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextpointtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:44:16 2026 GMT\n  hsts: false\ndomains:\n- domain: nextpointtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextpoint/refs/heads/main/security/nextpoint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Immunotherapy
- Precision Medicine
- Clinical Stage
- Drug Development
- Healthcare
- Life Sciences
---
