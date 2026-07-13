---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bundestag.de
  spf: true
hosts:
- cert_expires: Aug 24 07:06:31 2026 GMT
  host: dip.bundestag.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deutscher Bundestag Dip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutscher Bundestag DIP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deutscher Bundestag DIP
provider_slug: deutscher-bundestag-dip
slug: deutscher-bundestag-dip-domain-security
source_filename: deutscher-bundestag-dip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dip.bundestag.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:06:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bundestag.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutscher-bundestag-dip/refs/heads/main/security/deutscher-bundestag-dip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Public APIs
---
