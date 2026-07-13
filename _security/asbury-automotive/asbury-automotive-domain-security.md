---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asburyauto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clicklane.com
  spf: true
hosts:
- cert_expires: Sep 29 06:29:13 2026 GMT
  host: www.asburyauto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 06:47:11 2026 GMT
  host: www.clicklane.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asbury Automotive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asbury Automotive Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asbury Automotive Group
provider_slug: asbury-automotive
slug: asbury-automotive-domain-security
source_filename: asbury-automotive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asburyauto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:29:13 2026 GMT\n  hsts: null\n- host: www.clicklane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:47:11 2026 GMT\n  hsts: null\ndomains:\n- domain: asburyauto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: clicklane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asbury-automotive/refs/heads/main/security/asbury-automotive-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Dealerships
- Retail
- Vehicles
- Fortune 500
---
