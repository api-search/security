---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cormint.com
  spf: true
hosts:
- cert_expires: Dec 28 01:49:17 2026 GMT
  host: www.cormint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cormintdatasystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cormintdatasystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cormintdatasystems
provider_slug: cormintdatasystems
slug: cormintdatasystems-domain-security
source_filename: cormintdatasystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cormint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 01:49:17 2026 GMT\n  hsts: false\ndomains:\n- domain: cormint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cormintdatasystems/refs/heads/main/security/cormintdatasystems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- DataCenter
- BitcoinMining
- PowerInfrastructure
- Artificial Intelligence
---
