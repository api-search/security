---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 1social.dev
  spf: false
hosts:
- cert_expires: Dec 17 15:12:03 2026 GMT
  host: 1social.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1Social Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Social, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: 1Social
provider_slug: 1social-dev
slug: 1social-dev-domain-security
source_filename: 1social-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 1social.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:12:03 2026 GMT\n  hsts: false\ndomains:\n- domain: 1social.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/1social-dev/security/1social-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media
- AI Integration
- Automation
- Content Publishing
- ChatGPT
---
