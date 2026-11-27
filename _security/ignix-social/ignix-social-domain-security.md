---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ignix.social
  spf: true
hosts:
- cert_expires: Dec 29 18:02:33 2026 GMT
  host: ignix.social
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ignix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ignix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ignix
provider_slug: ignix-social
slug: ignix-social-domain-security
source_filename: ignix-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ignix.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 18:02:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ignix.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ignix-social/security/ignix-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Marketing
- Automation
- Software-as-a-Service
- Communications
---
