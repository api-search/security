---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: convergentrx.com
  spf: true
hosts:
- cert_expires: Oct 30 19:37:09 2026 GMT
  host: convergentrx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convergent Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convergent Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Convergent Therapeutics
provider_slug: convergent-therapeutics
slug: convergent-therapeutics-domain-security
source_filename: convergent-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convergentrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 19:37:09 2026 GMT\n  hsts: null\ndomains:\n- domain: convergentrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convergent-therapeutics/refs/heads/main/security/convergent-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Radiopharmaceuticals
- Clinical Trials
- Life Sciences
- Healthcare
---
