---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaizenlabs.co
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.kaizenlabs.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaizen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaizen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaizen
provider_slug: kaizen
slug: kaizen-domain-security
source_filename: kaizen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaizenlabs.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kaizenlabs.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaizen/refs/heads/main/security/kaizen-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud Saas
- Government
- GovTech
- Civic Technology
- Public Sector
- Permitting
- Payments
- Recreation
- Parking
- Transit
---
