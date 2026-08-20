---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: poptin.com
  spf: true
hosts:
- cert_expires: Oct  2 15:44:44 2026 GMT
  host: poptin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Poptin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poptin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Poptin
provider_slug: poptin
slug: poptin-domain-security
source_filename: poptin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: poptin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:44:44 2026 GMT\n  hsts: false\ndomains:\n- domain: poptin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poptin/refs/heads/main/security/poptin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Email Marketing
- Marketing Automation
- Lead Generation
- Conversion Optimization
- Forms
- Popups
- Contact Management
- Webhook
- E-Commerce
- Software-as-a-Service
---
