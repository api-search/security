---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: santos.com
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: santos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Santos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Santos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Santos
provider_slug: santos
slug: santos-domain-security
source_filename: santos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: santos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: santos.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santos/refs/heads/main/security/santos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Energy
- Oil and Gas
- Natural Gas
- LNG
- Australia
---
