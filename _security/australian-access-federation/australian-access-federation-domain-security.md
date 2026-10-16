---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aaf.edu.au
  spf: true
hosts:
- cert_expires: Nov 13 22:25:49 2026 GMT
  host: aaf.edu.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Australian Access Federation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Access Federation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Australian Access Federation
provider_slug: australian-access-federation
slug: australian-access-federation-domain-security
source_filename: australian-access-federation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaf.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 22:25:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aaf.edu.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-access-federation/refs/heads/main/security/australian-access-federation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Education
- Research
- Federation
---
