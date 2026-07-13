---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pool.com
  spf: true
hosts:
- cert_expires: Aug 17 05:42:34 2026 GMT
  host: www.pool.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Pool
provider_slug: pool
slug: pool-domain-security
source_filename: pool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 05:42:34 2026 GMT\n  hsts: false\ndomains:\n- domain: pool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pool/refs/heads/main/security/pool-domain-security.yml
summary_line: TLSv1.3
tags:
- Domains
- Web3
- Registrar
- Naming
- Fortune 1000
---
