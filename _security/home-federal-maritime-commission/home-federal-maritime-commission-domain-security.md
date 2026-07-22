---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fmc.gov
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.fmc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Home Federal Maritime Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Maritime Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Federal Maritime Commission
provider_slug: home-federal-maritime-commission
slug: home-federal-maritime-commission-domain-security
source_filename: home-federal-maritime-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fmc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fmc.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/home-federal-maritime-commission/refs/heads/main/security/home-federal-maritime-commission-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- Maritime
- Regulation
- Shipping
---
