---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sidechef.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: scgrocery.net
  spf: false
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.sidechef.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 07:31:06 2026 GMT
  host: business.sidechef.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.scgrocery.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidechef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SideChef, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SideChef
provider_slug: sidechef
slug: sidechef-domain-security
source_filename: sidechef-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sidechef.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business.sidechef.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:31:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.scgrocery.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sidechef.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: scgrocery.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidechef/refs/heads/main/security/sidechef-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food
- Recipes
- Retail
- Grocery
- Commerce
- Advertising
- Content
- Widgets
- Artificial Intelligence
- Nutrition
- Media
---
