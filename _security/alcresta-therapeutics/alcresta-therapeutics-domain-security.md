---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alcresta.com
  spf: true
hosts:
- cert_expires: Sep 18 00:46:40 2026 GMT
  host: www.alcresta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alcresta Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alcresta Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alcresta Therapeutics
provider_slug: alcresta-therapeutics
slug: alcresta-therapeutics-domain-security
source_filename: alcresta-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alcresta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 00:46:40 2026 GMT\n  hsts: false\ndomains:\n- domain: alcresta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alcresta-therapeutics/refs/heads/main/security/alcresta-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Pharmaceuticals
- Rare Disease
- Enzyme Therapy
- Enteral Nutrition
- Digestive Health
- Medical Device
- Life Sciences
---
