---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mercybio.com
  spf: true
hosts:
- cert_expires: Nov 10 14:57:15 2026 GMT
  host: mercybio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercy Bioanalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercy BioAnalytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mercy BioAnalytics
provider_slug: mercy-bioanalytics
slug: mercy-bioanalytics-domain-security
source_filename: mercy-bioanalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mercybio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:57:15 2026 GMT\n  hsts: false\ndomains:\n- domain: mercybio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercy-bioanalytics/refs/heads/main/security/mercy-bioanalytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health
- Diagnostics
- Biotechnology
- Life Sciences
- Cancer Screening
- Liquid Biopsy
- Laboratory
---
