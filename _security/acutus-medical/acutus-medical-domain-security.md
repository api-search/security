---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: acutus.com
  mx: true
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:spf.sendinblue.com include:_spf.salesforce.com ip4:160.72.29.227 ip4:161.38.194.251 -all
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: acutusmedical.com
  mx: true
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:sharepointonline.com include:spf.sendinblue.com ip4:160.72.29.227 -all
hosts:
- cert_expires: null
  host: acutus.com
  hsts: null
  hsts_max_age: null
  https: false
  https_error: no A record (DNS NOERROR, zero answers) — no TCP/443 endpoint to handshake
  tls_version: null
- cert_expires: null
  host: www.acutusmedical.com
  hsts: null
  hsts_max_age: null
  https: false
  https_error: NXDOMAIN
  tls_version: null
- cert_expires: null
  host: acutusmedical.com
  hsts: null
  hsts_max_age: null
  https: false
  https_error: no A record (DNS NOERROR, zero answers) — no TCP/443 endpoint to handshake
  tls_version: null
- cert_expires: null
  host: ir.acutusmedical.com
  hsts: null
  hsts_max_age: null
  https: false
  https_error: NXDOMAIN — the investor-relations host named in the company's own press releases no longer resolves
  tls_version: null
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Acutus Medical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acutus Medical, Inc., probed live across 4 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Acutus Medical, Inc.
provider_slug: acutus-medical
slug: acutus-medical-domain-security
source_filename: acutus-medical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  Live DNS/TLS probes of every registrable domain Acutus Medical, Inc. owns (acutus.com and\n  acutusmedical.com) on 2026-09-06. No apis.yml Website/Portal host and no OpenAPI servers[] host\n  exist to probe, because the company no longer publishes a web surface — both zones are delegated\n  to Cloudflare nameservers and serve mail records only.\nnote: >-\n  Neither apex resolves to an address: acutus.com answers NOERROR with zero A records and\n  www.acutusmedical.com answers NXDOMAIN, so no TLS handshake is possible and HSTS cannot be\n  observed. The zones are not empty — both still carry Microsoft 365 MX records\n  (acutus-com.mail.protection.outlook.com / acutusmedical-com.mail.protection.outlook.com), a\n  secondary MX at vor.acutusmedical.com, and a hard-fail SPF record, so corporate email continues\n  to route while the public web presence has been withdrawn. Neither domain publishes DNSSEC, CAA\n  or a DMARC record;\
  \ SPF without DMARC leaves the mail posture unenforced.\nhosts:\n- host: acutus.com\n  https: false\n  https_error: no A record (DNS NOERROR, zero answers) — no TCP/443 endpoint to handshake\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  hsts_max_age: null\n- host: www.acutusmedical.com\n  https: false\n  https_error: NXDOMAIN\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  hsts_max_age: null\n- host: acutusmedical.com\n  https: false\n  https_error: no A record (DNS NOERROR, zero answers) — no TCP/443 endpoint to handshake\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  hsts_max_age: null\n- host: ir.acutusmedical.com\n  https: false\n  https_error: NXDOMAIN — the investor-relations host named in the company's own press releases\n    no longer resolves\n  tls_version: null\n  cert_expires: null\n  hsts: null\n  hsts_max_age: null\ndomains:\n- domain: acutus.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com\
  \ include:spf.sendinblue.com include:_spf.salesforce.com\n    ip4:160.72.29.227 ip4:161.38.194.251 -all\n  dmarc: false\n  dmarc_policy: null\n  mx: true\n- domain: acutusmedical.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:sharepointonline.com include:spf.sendinblue.com\n    ip4:160.72.29.227 -all\n  dmarc: false\n  dmarc_policy: null\n  mx: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acutus-medical/refs/heads/main/security/acutus-medical-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Electrophysiology
- Cardiac Ablation
- Cardiac Mapping
- Contract Manufacturing
---
