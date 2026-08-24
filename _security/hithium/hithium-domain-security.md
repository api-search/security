---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hithium.com
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: hero-ee.com
  spf: false
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.hithium.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: en.hithium.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 10 10:02:23 2027 GMT
  host: www.hero-ee.com
  hsts: max-age=31536000; includeSubDomains; preload
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hithium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hithium, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hithium
provider_slug: hithium
slug: hithium-domain-security
source_filename: hithium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every HiTHIUM-controlled host (no API hosts exist)\nhosts:\n- host: www.hithium.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: en.hithium.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\n- host: www.hero-ee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:02:23 2027 GMT\n  hsts: max-age=31536000; includeSubDomains; preload\ndomains:\n- domain: hithium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hero-ee.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\nnote: www.hithium.com and en.hithium.com serve TLS 1.2 with no HSTS header; the HeroEE brand site www.hero-ee.com\n  serves TLS 1.3 with a full HSTS preload directive. Neither registrable domain is DNSSEC-signed and neither\n  publishes\
  \ a CAA record. hithium.com publishes SPF and a DMARC record at p=quarantine; hero-ee.com publishes\n  neither, so its domain can be spoofed in email. No API hosts exist to probe.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hithium/refs/heads/main/security/hithium-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Energy Storage
- Battery
- Lithium Iron Phosphate
- Renewable Energy
- Utilities
- Manufacturing
- Hardware
- Industrial Control Systems
---
