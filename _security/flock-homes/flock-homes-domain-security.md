---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flockhomes.com
  spf: true
hosts:
- cert_expires: Oct 14 15:33:49 2026 GMT
  host: www.flockhomes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flock Homes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flock Homes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flock Homes
provider_slug: flock-homes
slug: flock-homes-domain-security
source_filename: flock-homes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flockhomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flockhomes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flock-homes/refs/heads/main/security/flock-homes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- Investment
- Property Management
- 721 Exchange
- Fund
- Proptech
- Fintech
---
