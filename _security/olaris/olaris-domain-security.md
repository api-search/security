---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: myolaris.com
  spf: true
hosts:
- cert_expires: Sep 17 16:58:42 2026 GMT
  host: www.myolaris.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olaris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Olaris
provider_slug: olaris
slug: olaris-domain-security
source_filename: olaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.myolaris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: myolaris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olaris/refs/heads/main/security/olaris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Diagnostics
- Precision Medicine
- Metabolomics
- Machine Learning
- Biomarkers
- Laboratory
- Transplant
- Life Sciences
---
