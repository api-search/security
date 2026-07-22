---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: verisian.com
  spf: true
hosts:
- cert_expires: Sep 29 16:54:46 2026 GMT
  host: verisian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verisian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verisian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Verisian
provider_slug: verisian
slug: verisian-domain-security
source_filename: verisian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verisian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:54:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: verisian.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisian/refs/heads/main/security/verisian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Clinical Trials
- Life Sciences
- Artificial Intelligence
- Pharmaceutical
- Regulatory Submissions
- Data Validation
- Healthcare
---
