---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hedvig.com
  spf: true
hosts:
- cert_expires: Sep 25 13:05:13 2026 GMT
  host: hedvig.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hedvig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hedvig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hedvig
provider_slug: hedvig
slug: hedvig-domain-security
source_filename: hedvig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hedvig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:05:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hedvig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedvig/refs/heads/main/security/hedvig-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurtech
- Insurance
- Sweden
- Consumer
- Mobile
- Home Insurance
- Pet Insurance
---
