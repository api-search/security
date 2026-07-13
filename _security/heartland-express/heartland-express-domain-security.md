---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heartlandexpress.com
  spf: true
hosts:
- cert_expires: Aug 18 20:55:16 2026 GMT
  host: www.heartlandexpress.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: developer.heartlandexpress.com
  https: false
- host: api.heartlandexpress.com
  https: false
kind: domain-security
layout: security
method: probed
name: Heartland Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heartland Express, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heartland Express
provider_slug: heartland-express
slug: heartland-express-domain-security
source_filename: heartland-express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heartlandexpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 20:55:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.heartlandexpress.com\n  https: false\n- host: api.heartlandexpress.com\n  https: false\ndomains:\n- domain: heartlandexpress.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heartland-express/refs/heads/main/security/heartland-express-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trucking
- Transportation
- Logistics
---
