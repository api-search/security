---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inegi.org.mx
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.inegi.org.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Mexico Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Mexico, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Government, Mexico
provider_slug: open-government-mexico
slug: open-government-mexico-domain-security
source_filename: open-government-mexico-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inegi.org.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: inegi.org.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-mexico/refs/heads/main/security/open-government-mexico-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
