---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jefferies.com
  spf: true
hosts:
- cert_expires: Aug 28 11:17:11 2026 GMT
  host: www.jefferies.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leucadia National Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leucadia National, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leucadia National
provider_slug: leucadia-national
slug: leucadia-national-domain-security
source_filename: leucadia-national-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jefferies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:17:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jefferies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leucadia-national/refs/heads/main/security/leucadia-national-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Holding Company
- Investment Banking
- Financial Services
- Historical
- Fortune 500
---
