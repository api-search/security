---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ansunbiopharma.com
  spf: true
hosts:
- cert_expires: Dec  2 17:01:20 2026 GMT
  host: www.ansunbiopharma.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ansun Biopharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansun Biopharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ansun Biopharma
provider_slug: ansun-biopharma
slug: ansun-biopharma-domain-security
source_filename: ansun-biopharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ansunbiopharma.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 17:01:20 2026 GMT\n  hsts: false\ndomains:\n- domain: ansunbiopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansun-biopharma/refs/heads/main/security/ansun-biopharma-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Biotechnology
- Biopharmaceutical
- Life Sciences
- Clinical Trials
- Antivirals
- Health
- Drug Development
- San Diego
---
