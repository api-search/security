---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: summeros.com
  spf: true
hosts:
- cert_expires: Aug 24 18:55:08 2026 GMT
  host: www.summeros.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Summer 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Summer 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Summer 2
provider_slug: summer-2
slug: summer-2-domain-security
source_filename: summer-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.summeros.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:55:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: summeros.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/summer-2/refs/heads/main/security/summer-2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Short-Term Rental
- Vacation Rental
- Property Management
- Analytics
- Revenue Management
- Proptech
- Artificial Intelligence
- Market Intelligence
---
