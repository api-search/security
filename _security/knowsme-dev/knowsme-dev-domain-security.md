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
  domain: knowsme.dev
  spf: false
hosts:
- cert_expires: Dec 22 23:25:03 2026 GMT
  host: knowsme.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: knowsme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for knowsme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: knowsme
provider_slug: knowsme-dev
slug: knowsme-dev-domain-security
source_filename: knowsme-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knowsme.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:25:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: knowsme.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/knowsme-dev/security/knowsme-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Privacy
- Ghana
---
