---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lecollectionist.com
  spf: true
hosts:
- cert_expires: Aug 24 06:01:39 2026 GMT
  host: lecollectionist.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Le Collectionist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Le Collectionist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Le Collectionist
provider_slug: le-collectionist
slug: le-collectionist-domain-security
source_filename: le-collectionist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lecollectionist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:01:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lecollectionist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/le-collectionist/refs/heads/main/security/le-collectionist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Travel
- Hospitality
- Luxury
- Villa Rental
- Concierge
- France
---
