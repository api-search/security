---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: condor.energy
  spf: true
hosts:
- cert_expires: Sep  6 02:36:35 2026 GMT
  host: www.condor.energy
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Condor Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Condor Energy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Condor Energy
provider_slug: condor-energy
slug: condor-energy-domain-security
source_filename: condor-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.condor.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 02:36:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: condor.energy\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/condor-energy/refs/heads/main/security/condor-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Energy Procurement
- Energy Management
- Sustainability
- Data Centers
- Price Risk Management
- Artificial Intelligence
- Analytics
---
