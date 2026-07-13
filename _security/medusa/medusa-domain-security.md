---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: medusajs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-medusa-instance.com
  spf: false
hosts:
- cert_expires: Aug 23 12:37:45 2026 GMT
  host: docs.medusajs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-medusa-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Medusa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medusa, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Medusa
provider_slug: medusa
slug: medusa-domain-security
source_filename: medusa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.medusajs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 12:37:45 2026 GMT\n  hsts: false\n- host: your-medusa-instance.com\n  https: false\ndomains:\n- domain: medusajs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-medusa-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medusa/refs/heads/main/security/medusa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Headless Commerce
- Open Source
- GraphQL
- Node.js
---
