---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getbento.com
  spf: true
hosts:
- cert_expires: Aug 17 16:33:31 2026 GMT
  host: www.getbento.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bentobox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BentoBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BentoBox
provider_slug: bentobox
slug: bentobox-domain-security
source_filename: bentobox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getbento.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: getbento.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bentobox/refs/heads/main/security/bentobox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Online Ordering
- Websites
- Commerce
- Integrations
- Payments
- Reservations
- Delivery
- Hospitality
---
