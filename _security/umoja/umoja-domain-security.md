---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: umoja-biopharma.com
  spf: true
hosts:
- cert_expires: Sep 16 18:58:36 2026 GMT
  host: www.umoja-biopharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umoja Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umoja Biopharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Umoja Biopharma
provider_slug: umoja
slug: umoja-domain-security
source_filename: umoja-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.umoja-biopharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:58:36 2026 GMT\n  hsts: false\ndomains:\n- domain: umoja-biopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umoja/refs/heads/main/security/umoja-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Immunotherapy
- CAR-T
- Cell Therapy
- Oncology
- Gene Therapy
- Healthcare
---
