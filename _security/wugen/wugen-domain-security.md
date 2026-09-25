---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloteratx.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wugen.com
  spf: true
hosts:
- cert_expires: Sep 10 22:59:46 2026 GMT
  host: alloteratx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 19:13:07 2026 GMT
  host: wugen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Wugen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wugen, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wugen
provider_slug: wugen
slug: wugen-domain-security
source_filename: wugen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alloteratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:59:46 2026 GMT\n  hsts: false\n- host: wugen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 19:13:07 2026 GMT\n  hsts: false\ndomains:\n- domain: alloteratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wugen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wugen/refs/heads/main/security/wugen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Cell Therapy
- Oncology
- Life Sciences
- Pharmaceuticals
- Clinical Trials
- Cart
- CRISPR
- Immunotherapy
- Research
- Content
---
