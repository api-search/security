---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aramisauto.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aramis.group
  spf: true
hosts:
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: www.aramisauto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 01:02:49 2026 GMT
  host: schemas.aramis.group
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.aramisauto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aramisauto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AramisAuto, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AramisAuto
provider_slug: aramisauto
slug: aramisauto-domain-security
source_filename: aramisauto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aramisauto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: false\n- host: schemas.aramis.group\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:02:49 2026 GMT\n  hsts: false\n- host: api.aramisauto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aramisauto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aramis.group\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aramisauto/refs/heads/main/security/aramisauto-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Automotive
- E-Commerce
- Used Cars
- Vehicle Data
- Marketplace
- Retail
- Auto Finance
- France
- JSON Schema
---
