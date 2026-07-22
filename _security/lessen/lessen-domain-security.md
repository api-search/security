---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lessen.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lessenpro.com
  spf: true
hosts:
- cert_expires: Oct  3 16:44:19 2026 GMT
  host: www.lessen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 18:03:19 2026 GMT
  host: status.lessen.com
  hsts: false
  https: true
  note: status page CNAME -> status.hyperping.io (Hyperping-hosted)
  tls_version: TLSv1.2
- cert_expires: Sep 20 19:26:57 2026 GMT
  host: www.lessenpro.com
  hsts: false
  https: true
  note: Lessen Pro affiliate/contractor product on a separate registrable domain
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lessen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lessen, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lessen
provider_slug: lessen
slug: lessen-domain-security
source_filename: lessen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lessen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:44:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: status.lessen.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 18:03:19 2026 GMT\n  hsts: false\n  note: status page CNAME -> status.hyperping.io (Hyperping-hosted)\n- host: www.lessenpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:26:57 2026 GMT\n  hsts: false\n  note: Lessen Pro affiliate/contractor product on a separate registrable domain\ndomains:\n- domain: lessen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: lessenpro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lessen/refs/heads/main/security/lessen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- Property Management
- Facilities Management
- Field Service Management
- Work Order Management
- Maintenance
- Marketplace
- Construction
---
