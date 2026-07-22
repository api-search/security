---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trishulatx.com
  spf: true
hosts:
- cert_expires: Sep 25 12:02:13 2026 GMT
  host: www.trishulatx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trishula Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trishula Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trishula Therapeutics
provider_slug: trishula-therapeutics
slug: trishula-therapeutics-domain-security
source_filename: trishula-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trishulatx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:02:13 2026 GMT\n  hsts: false\ndomains:\n- domain: trishulatx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trishula-therapeutics/refs/heads/main/security/trishula-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Immuno-Oncology
- Pharmaceuticals
- Cancer
- Therapeutics
- Clinical Stage
- Immunotherapy
---
