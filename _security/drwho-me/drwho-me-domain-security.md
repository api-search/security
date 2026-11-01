---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: drwho.me
  spf: false
hosts:
- cert_expires: Jan  9 20:22:07 2027 GMT
  host: drwho.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Drwho Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for drwho-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: drwho-me
provider_slug: drwho-me
slug: drwho-me-domain-security
source_filename: drwho-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drwho.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 20:22:07 2027 GMT\n  hsts: false\ndomains:\n- domain: drwho.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/drwho-me/security/drwho-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Tools
- Free
- DNS
- Email
- Browser
---
