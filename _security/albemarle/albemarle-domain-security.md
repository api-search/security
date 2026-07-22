---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: albemarle.com
  spf: true
hosts:
- cert_expires: Oct  7 03:48:09 2026 GMT
  host: www.albemarle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Albemarle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Albemarle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Albemarle
provider_slug: albemarle
slug: albemarle-domain-security
source_filename: albemarle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.albemarle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:09 2026 GMT\n  hsts: false\ndomains:\n- domain: albemarle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/albemarle/refs/heads/main/security/albemarle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Chemicals
- Lithium
- Bromine
- Energy Storage
- Electric Vehicles
- Specialty Chemicals
- Pharmaceuticals
- Sustainability
- Materials Science
- Manufacturing
- Fortune 1000
---
