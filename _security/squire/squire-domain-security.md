---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getsquire.com
  spf: true
hosts:
- cert_expires: Oct 13 13:16:57 2026 GMT
  host: getsquire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Squire
provider_slug: squire
slug: squire-domain-security
source_filename: squire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsquire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:16:57 2026 GMT\n  hsts: false\ndomains:\n- domain: getsquire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squire/refs/heads/main/security/squire-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Booking
- Scheduling
- Payments
- Point of Sale
- Barbershop
- SaaS
- Small Business
---
