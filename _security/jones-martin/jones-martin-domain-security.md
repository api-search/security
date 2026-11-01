---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jonesandmartinauctions.com
  spf: true
hosts:
- cert_expires: Dec 10 08:16:15 2026 GMT
  host: jonesandmartinauctions.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jones Martin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jones, Martin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jones, Martin
provider_slug: jones-martin
slug: jones-martin-domain-security
source_filename: jones-martin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jonesandmartinauctions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 08:16:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: jonesandmartinauctions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/jones-martin/security/jones-martin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Auctions
- Real Estate
- Collectibles
- Pennsylvania
---
