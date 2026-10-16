---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cntxt.tech
  spf: true
hosts:
- cert_expires: Dec  3 10:27:08 2026 GMT
  host: cntxt.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cntxt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NBULA - AI As A Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NBULA - AI As A Service
provider_slug: cntxt
slug: cntxt-domain-security
source_filename: cntxt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cntxt.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 10:27:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cntxt.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cntxt/refs/heads/main/security/cntxt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Data
- Arabic
- Enterprise
---
