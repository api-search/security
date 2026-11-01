---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zosanopharma.com
  spf: false
hosts:
- cert_expires: Jan  3 11:42:41 2027 GMT
  host: www.zosanopharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zosano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zosano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zosano
provider_slug: zosano
slug: zosano-domain-security
source_filename: zosano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zosanopharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 11:42:41 2027 GMT\n  hsts: false\ndomains:\n- domain: zosanopharma.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zosano/security/zosano-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
