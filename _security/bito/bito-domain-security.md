---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bito.ai
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: bito.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bito, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bito
provider_slug: bito
slug: bito-domain-security
source_filename: bito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bito.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bito.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bito/refs/heads/main/security/bito-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Developer Tools
- SaaS
- Machine Learning
---
