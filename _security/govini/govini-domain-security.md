---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: govini.com
  spf: true
hosts:
- cert_expires: Sep 14 01:28:54 2026 GMT
  host: www.govini.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govini Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Govini, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Govini
provider_slug: govini
slug: govini-domain-security
source_filename: govini-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.govini.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:28:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govini.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govini/refs/heads/main/security/govini-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Defense
- Government
- National Security
- Defense Acquisition
- Analytics
- Supply Chain
---
