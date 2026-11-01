---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quuu.co
  spf: true
hosts:
- cert_expires: Dec  1 18:19:20 2026 GMT
  host: quuu.co
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Quuu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quuu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quuu
provider_slug: quuu
slug: quuu-domain-security
source_filename: quuu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quuu.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 18:19:20 2026 GMT\n  hsts: false\ndomains:\n- domain: quuu.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/quuu/security/quuu-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- AI
- Social Media
- Automation
- Marketing
---
