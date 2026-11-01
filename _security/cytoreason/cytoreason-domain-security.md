---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cytoreason.com
  spf: true
hosts:
- cert_expires: Jan 12 16:40:52 2027 GMT
  host: www.cytoreason.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cytoreason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cytoreason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cytoreason
provider_slug: cytoreason
slug: cytoreason-domain-security
source_filename: cytoreason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cytoreason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 16:40:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cytoreason.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cytoreason/security/cytoreason-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biotechnology
- Artificial Intelligence
- Drug Discovery
- Computational Biology
- Haifa
---
