---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vantage-dc.com
  spf: true
hosts:
- cert_expires: Dec 16 01:11:39 2026 GMT
  host: vantage-dc.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vantage Data Centers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantage Data Centers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vantage Data Centers
provider_slug: vantage-data-centers
slug: vantage-data-centers-domain-security
source_filename: vantage-data-centers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vantage-dc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 01:11:39 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: vantage-dc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vantage-data-centers/security/vantage-data-centers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Centers
- Build-to-Suit
- Cloud Infrastructure
- Sustainability
- Power
- Cooling
- Security
---
