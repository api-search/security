---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: returnpath.com
  spf: true
hosts:
- cert_expires: Sep 29 12:53:58 2026 GMT
  host: www.returnpath.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Return Path Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Return Path, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Return Path
provider_slug: return-path
slug: return-path-domain-security
source_filename: return-path-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.returnpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:53:58 2026 GMT\n  hsts: null\ndomains:\n- domain: returnpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/return-path/refs/heads/main/security/return-path-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Martech
- Email
- Email Deliverability
- Email Marketing
- Sender Reputation
- Inbox Placement
- Deliverability
---
