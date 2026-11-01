---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Nov 27 19:48:08 2026 GMT
  host: saash-gateway.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saash Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAASH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAASH
provider_slug: saash-gateway
slug: saash-gateway-domain-security
source_filename: saash-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saash-gateway.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saash-gateway/security/saash-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
