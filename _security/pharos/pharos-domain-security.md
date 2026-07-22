---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pharos.health
  spf: true
hosts:
- cert_expires: Oct 16 11:39:53 2026 GMT
  host: pharos.health
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pharos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pharos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pharos
provider_slug: pharos
slug: pharos-domain-security
source_filename: pharos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pharos.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: pharos.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pharos/refs/heads/main/security/pharos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Patient Safety
- Hospitals
- Quality Improvement
- Health Technology
- Clinical
---
