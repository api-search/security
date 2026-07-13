---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glofox.com
  spf: true
hosts:
- cert_expires: Sep  9 23:56:28 2026 GMT
  host: www.glofox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: apidocs-plat.aws.glofox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: gf-api.aws.glofox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glofox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glofox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Glofox
provider_slug: glofox
slug: glofox-domain-security
source_filename: glofox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.glofox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:56:28 2026 GMT\n  hsts: false\n- host: apidocs-plat.aws.glofox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\n- host: gf-api.aws.glofox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: glofox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glofox/refs/heads/main/security/glofox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Gym Management
- Boutique Fitness
- Class Scheduling
- Bookings
- Memberships
- Leads
- ABC Fitness
- CDC Webhooks
---
