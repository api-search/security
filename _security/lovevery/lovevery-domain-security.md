---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lovevery.com
  spf: true
hosts:
- cert_expires: Sep 30 02:02:51 2026 GMT
  host: lovevery.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lovevery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lovevery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lovevery
provider_slug: lovevery
slug: lovevery-domain-security
source_filename: lovevery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lovevery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lovevery.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovevery/refs/heads/main/security/lovevery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-commerce
- Retail
- Children
- Education
- Subscription
---
