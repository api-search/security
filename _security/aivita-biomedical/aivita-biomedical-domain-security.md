---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aivitabiomedical.com
  spf: true
hosts:
- cert_expires: Nov 28 21:49:30 2026 GMT
  host: aivitabiomedical.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aivita Biomedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AiVita Biomedical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AiVita Biomedical
provider_slug: aivita-biomedical
slug: aivita-biomedical-domain-security
source_filename: aivita-biomedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aivitabiomedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 21:49:30 2026 GMT\n  hsts: false\ndomains:\n- domain: aivitabiomedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aivita-biomedical/refs/heads/main/security/aivita-biomedical-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Personalized Medicine
- Cancer
- Infectious Disease
- Stem Cell
---
