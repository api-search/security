---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kymeratx.com
  spf: true
hosts:
- cert_expires: Sep 25 05:29:14 2026 GMT
  host: www.kymeratx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kymera Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kymera Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kymera Therapeutics
provider_slug: kymera-therapeutics
slug: kymera-therapeutics-domain-security
source_filename: kymera-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kymeratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:29:14 2026 GMT\n  hsts: false\ndomains:\n- domain: kymeratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kymera-therapeutics/refs/heads/main/security/kymera-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotech
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Targeted Protein Degradation
- Immunology
- Oncology
- Clinical Trials
- Healthcare
---
