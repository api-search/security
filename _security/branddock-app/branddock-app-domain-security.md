---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: branddock.app
  spf: false
hosts:
- cert_expires: Dec 16 07:20:56 2026 GMT
  host: branddock.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Branddock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branddock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Branddock
provider_slug: branddock-app
slug: branddock-app-domain-security
source_filename: branddock-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branddock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 07:20:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: branddock.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/branddock-app/security/branddock-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Branding
- Collaboration
- Automation
---
