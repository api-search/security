---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bahn.de
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: bahn.de
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deutsche Bahn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deutsche Bahn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deutsche Bahn
provider_slug: deutsche-bahn
slug: deutsche-bahn-domain-security
source_filename: deutsche-bahn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bahn.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: bahn.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deutsche-bahn/refs/heads/main/security/deutsche-bahn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Transportation
- Railways
- Travel
- Germany
---
