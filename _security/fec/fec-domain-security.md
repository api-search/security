---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fec.gov
  spf: true
hosts:
- cert_expires: Aug 18 14:21:16 2026 GMT
  host: api.open.fec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FEC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FEC
provider_slug: fec
slug: fec-domain-security
source_filename: fec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.open.fec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 14:21:16 2026 GMT\n  hsts: null\ndomains:\n- domain: fec.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fec/refs/heads/main/security/fec-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
