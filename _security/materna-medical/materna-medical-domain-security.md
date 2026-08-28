---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: maternamedical.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hellomilli.com
  spf: true
hosts:
- cert_expires: Sep 27 11:33:17 2026 GMT
  host: www.maternamedical.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cdn: cloudflare
  cert_expires: Oct 28 17:51:22 2026 GMT
  host: www.hellomilli.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Materna Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materna Medical, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Materna Medical
provider_slug: materna-medical
slug: materna-medical-domain-security
source_filename: materna-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (www.maternamedical.com corporate site, www.hellomilli.com Milli storefront)\nnote: >-\n  Materna Medical publishes no API host, so there is no API surface to probe here; these are the\n  two public web properties named in apis.yml. www.maternamedical.com is WordPress on WP Engine;\n  www.hellomilli.com is WooCommerce behind Cloudflare. Neither domain publishes DMARC enforcement\n  (hellomilli.com is p=none, maternamedical.com has no _dmarc record at all), neither publishes a\n  CAA record, and neither is DNSSEC-signed.\nhosts:\n- host: www.maternamedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:33:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.hellomilli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:51:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  cdn:\
  \ cloudflare\ndomains:\n- domain: maternamedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: hellomilli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materna-medical/refs/heads/main/security/materna-medical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health Care
- Medical Devices
- Women's Health
- Pelvic Health
- OBGYN
- Maternal Health
- Consumer Health
- Clinical Trials
- Medical Technology
---
