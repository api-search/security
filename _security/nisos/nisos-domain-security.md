---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nisos.com
  spf: true
hosts:
- cert_expires: Oct 13 20:47:03 2026 GMT
  host: nisos.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: api.ascend.nisos.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nisos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nisos, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nisos
provider_slug: nisos
slug: nisos-domain-security
source_filename: nisos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nisos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:47:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ascend.nisos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nisos.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nisos/refs/heads/main/security/nisos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Threat Intelligence
- Human Risk Management
- Insider Threat
- Executive Protection
- OSINT
- Digital Investigations
- Cybersecurity
- Adversary Attribution
- Employment Fraud
- Third-Party Risk
- Trust and Safety
- Dark Web Monitoring
- Managed Services
- Federal
---
