---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: l2l.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leading2lean.com
  spf: true
hosts:
- cert_expires: Sep 21 21:00:48 2026 GMT
  host: www.l2l.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: support.leading2lean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swipeguide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swipeguide, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Swipeguide
provider_slug: swipeguide
slug: swipeguide-domain-security
source_filename: swipeguide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.l2l.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: support.leading2lean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: l2l.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: leading2lean.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swipeguide/refs/heads/main/security/swipeguide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Work Instructions
- Frontline
- Shop Floor
- Maintenance
- Connected Worker
- Smart Manufacturing
- Industrial
---
