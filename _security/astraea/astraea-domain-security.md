---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryastraea.com
  spf: true
hosts:
- cert_expires: Sep 29 18:06:57 2026 GMT
  host: www.tryastraea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astraea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astraea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Astraea
provider_slug: astraea
slug: astraea-domain-security
source_filename: astraea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryastraea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:06:57 2026 GMT\n  hsts: false\ndomains:\n- domain: tryastraea.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astraea/refs/heads/main/security/astraea-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- Artificial Intelligence
- Biometrics
- Clinical Development
- Pharmaceutical
- CDISC
- Regulatory
---
