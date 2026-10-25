---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: superretailgroup.com.au
  spf: true
hosts:
- cert_expires: Dec 17 11:09:25 2026 GMT
  host: superretailgroup.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Super Retail Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Super Retail Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Super Retail Group
provider_slug: super-retail-group
slug: super-retail-group-domain-security
source_filename: super-retail-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superretailgroup.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 11:09:25 2026 GMT\n  hsts: false\ndomains:\n- domain: superretailgroup.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/super-retail-group/refs/heads/main/security/super-retail-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Retail
- Australia
- New Zealand
- Automotive
- Sporting Goods
- Outdoor
---
