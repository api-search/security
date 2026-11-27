---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortytwo.network
  spf: true
hosts:
- cert_expires: Feb  3 15:17:01 2027 GMT
  host: fortytwo.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 07:31:19 2027 GMT
  host: docs.fortytwo.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 11:20:31 2026 GMT
  host: api.fortytwo.network
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fortytwo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fortytwo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fortytwo
provider_slug: fortytwo-network
slug: fortytwo-network-domain-security
source_filename: fortytwo-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fortytwo.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 15:17:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fortytwo.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 07:31:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.fortytwo.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 11:20:31 2026 GMT\n  hsts: null\ndomains:\n- domain: fortytwo.network\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fortytwo-network/security/fortytwo-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Platform
- Open Source
---
