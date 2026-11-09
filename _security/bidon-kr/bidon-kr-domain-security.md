---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bidon.kr
  spf: false
hosts:
- cert_expires: Dec 22 06:15:28 2026 GMT
  host: bidon.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidon Kr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 비드온 BIDON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 비드온 BIDON
provider_slug: bidon-kr
slug: bidon-kr-domain-security
source_filename: bidon-kr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bidon.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:15:28 2026 GMT\n  hsts: false\ndomains:\n- domain: bidon.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bidon-kr/security/bidon-kr-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Procurement
- Marketplace
- Free
---
