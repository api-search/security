---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groupboss.io
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: groupboss.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groupboss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groupboss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groupboss
provider_slug: groupboss
slug: groupboss-domain-security
source_filename: groupboss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groupboss.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: groupboss.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupboss/refs/heads/main/security/groupboss-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lead Generation
- Marketing
- Marketing Automation
- Email Marketing
- CRM
- Social Media
- Community
- Browser Extension
- SaaS
---
