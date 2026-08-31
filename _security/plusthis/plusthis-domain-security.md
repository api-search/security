---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plusthis.com
  spf: true
hosts:
- cert_expires: Sep 29 12:26:47 2026 GMT
  host: plusthis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plusthis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlusThis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PlusThis
provider_slug: plusthis
slug: plusthis-domain-security
source_filename: plusthis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plusthis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:26:47 2026 GMT\n  hsts: false\ndomains:\n- domain: plusthis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plusthis/refs/heads/main/security/plusthis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing Automation
- Marketing
- CRM
- Sales
- No Code
- Automation
- Integration
- Webhook
- Email Marketing
- SMS
- Small Business
---
