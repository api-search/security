---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: limebike.com
  spf: true
hosts:
- cert_expires: Jan  4 22:15:49 2027 GMT
  host: www.limebike.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Limebike Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lime
provider_slug: limebike-com
slug: limebike-com-domain-security
source_filename: limebike-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.limebike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:15:49 2027 GMT\n  hsts: null\ndomains:\n- domain: limebike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/limebike-com/security/limebike-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
