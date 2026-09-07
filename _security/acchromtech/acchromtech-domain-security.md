---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acchrom-tech.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.acchrom-tech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acchromtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acchromtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Acchromtech
provider_slug: acchromtech
slug: acchromtech-domain-security
source_filename: acchromtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acchrom-tech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: acchrom-tech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acchromtech/refs/heads/main/security/acchromtech-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Chromatography
- Analytical Instruments
- Scientific Instruments
- Laboratory
- Life Sciences
- Manufacturing
- China
---
