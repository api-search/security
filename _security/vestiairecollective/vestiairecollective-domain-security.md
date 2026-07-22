---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vestiairecollective.com
  spf: true
hosts:
- cert_expires: Sep  7 03:46:10 2026 GMT
  host: www.vestiairecollective.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vestiairecollective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vestiairecollective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: vestiairecollective
provider_slug: vestiairecollective
slug: vestiairecollective-domain-security
source_filename: vestiairecollective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vestiairecollective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 03:46:10 2026 GMT\n  hsts: null\ndomains:\n- domain: vestiairecollective.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vestiairecollective/refs/heads/main/security/vestiairecollective-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fashion
- Luxury
- Marketplace
- Resale
- E-Commerce
- Circular Economy
- Second-Hand
---
