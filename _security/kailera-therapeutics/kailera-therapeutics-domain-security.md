---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kailera.com
  spf: true
hosts:
- cert_expires: Oct 17 03:12:09 2026 GMT
  host: www.kailera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kailera Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kailera Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kailera Therapeutics
provider_slug: kailera-therapeutics
slug: kailera-therapeutics-domain-security
source_filename: kailera-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kailera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 03:12:09 2026 GMT\n  hsts: null\ndomains:\n- domain: kailera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kailera-therapeutics/refs/heads/main/security/kailera-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Biotechnology
- Pharmaceuticals
- Obesity
- Metabolic Health
- GLP-1
- Clinical Stage
- Healthcare
---
