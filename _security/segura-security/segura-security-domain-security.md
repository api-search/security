---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: segura.security
  spf: true
hosts:
- cert_expires: Dec 17 00:36:12 2026 GMT
  host: www.segura.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Segura Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Segura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Segura
provider_slug: segura-security
slug: segura-security-domain-security
source_filename: segura-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.segura.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 00:36:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: segura.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/segura-security/refs/heads/main/security/segura-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
