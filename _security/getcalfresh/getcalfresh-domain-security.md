---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getcalfresh.org
  spf: true
hosts:
- cert_expires: Sep  4 20:48:14 2026 GMT
  host: www.getcalfresh.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getcalfresh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetCalFresh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GetCalFresh
provider_slug: getcalfresh
slug: getcalfresh-domain-security
source_filename: getcalfresh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcalfresh.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:48:14 2026 GMT\n  hsts: false\ndomains:\n- domain: getcalfresh.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getcalfresh/refs/heads/main/security/getcalfresh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Civic Tech
- Nonprofit
- Government
- Public Benefits
- SNAP
- Food Assistance
- California
---
