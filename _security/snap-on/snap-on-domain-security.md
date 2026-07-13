---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snapon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shopkeypro.com
  spf: true
hosts:
- cert_expires: Sep 23 13:41:37 2026 GMT
  host: www.snapon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: sbs.snapon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.shopkeypro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snap On Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snap-on, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snap-on
provider_slug: snap-on
slug: snap-on-domain-security
source_filename: snap-on-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.snapon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:41:37 2026 GMT\n  hsts: false\n- host: sbs.snapon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: www.shopkeypro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: snapon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: shopkeypro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snap-on/refs/heads/main/security/snap-on-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Diagnostics
- Electronic Parts Catalog
- Industrial Tools
- Manufacturing
- Repair Information
- Vehicle Repair
- Fortune 1000
---
