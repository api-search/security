---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: accelerant.ai
  spf: true
hosts:
- cert_expires: Oct 22 02:31:02 2026 GMT
  host: accelerant.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:13:15 2026 GMT
  host: docs.accelerant.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 02:31:02 2026 GMT
  host: api.accelerant.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accelerant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accelerant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Accelerant
provider_slug: accelerant
slug: accelerant-domain-security
source_filename: accelerant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accelerant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 02:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.accelerant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:13:15 2026 GMT\n  hsts: false\n- host: api.accelerant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 02:31:02 2026 GMT\n  hsts: null\ndomains:\n- domain: accelerant.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelerant/refs/heads/main/security/accelerant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- Specialty Insurance
- Underwriting
- Risk Management
- Reinsurance
- Marketplace
- Risk Scoring
- Financial Services
- Artificial Intelligence
---
