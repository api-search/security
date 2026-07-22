---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omass.com
  spf: true
hosts:
- cert_expires: Sep 29 18:39:45 2026 GMT
  host: omass.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omass Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OMass Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OMass Therapeutics
provider_slug: omass-therapeutics
slug: omass-therapeutics-domain-security
source_filename: omass-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: omass.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:39:45 2026 GMT\n  hsts: false\ndomains:\n- domain: omass.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omass-therapeutics/refs/heads/main/security/omass-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Mass Spectrometry
- Immunology
- Rare Diseases
---
