---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kniferiver.com
  spf: true
hosts:
- cert_expires: Sep 21 23:34:35 2026 GMT
  host: www.kniferiver.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:34:35 2026 GMT
  host: partner.kniferiver.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knife River Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knife River, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knife River
provider_slug: knife-river
slug: knife-river-domain-security
source_filename: knife-river-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kniferiver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: partner.kniferiver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:34:35 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kniferiver.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knife-river/refs/heads/main/security/knife-river-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Aggregates
- Concrete
- Asphalt
- Materials
- Infrastructure
---
