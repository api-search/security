---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getbooyah.com
  spf: true
hosts:
- cert_expires: Jan  7 08:54:01 2027 GMT
  host: getbooyah.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Booyah! Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Booyah!, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Booyah!
provider_slug: getbooyah-com
slug: getbooyah-com-domain-security
source_filename: getbooyah-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbooyah.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 08:54:01 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getbooyah.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/getbooyah-com/security/getbooyah-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- SEO
- Digital Agency
- Southeast Asia
---
