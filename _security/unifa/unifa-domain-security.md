---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unifa-e.com
  spf: true
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: unifa-e.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unifa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unifa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unifa
provider_slug: unifa
slug: unifa-domain-security
source_filename: unifa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unifa-e.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: unifa-e.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unifa/refs/heads/main/security/unifa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Childcare
- Education Technology
- Early Childhood Education
- SaaS
- Japan
- Internet of Things
- Artificial Intelligence
- Workforce Management
- Photo Sharing
---
