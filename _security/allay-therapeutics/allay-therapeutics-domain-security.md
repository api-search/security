---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allaytx.com
  spf: true
hosts:
- cert_expires: Oct 27 14:24:26 2026 GMT
  host: www.allaytx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Allay Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allay Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allay Therapeutics
provider_slug: allay-therapeutics
slug: allay-therapeutics-domain-security
source_filename: allay-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allaytx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 14:24:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: allaytx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allay-therapeutics/refs/heads/main/security/allay-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Pain Management
- Drug Delivery
- Non-Opioid
- Clinical Stage
- Health
- Life Sciences
- content-api
---
