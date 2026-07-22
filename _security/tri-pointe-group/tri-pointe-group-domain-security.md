---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tripointehomes.com
  spf: true
hosts:
- cert_expires: Aug 24 13:15:49 2026 GMT
  host: www.tripointehomes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tri Pointe Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tri Pointe Homes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tri Pointe Homes
provider_slug: tri-pointe-group
slug: tri-pointe-group-domain-security
source_filename: tri-pointe-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tripointehomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 13:15:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tripointehomes.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tri-pointe-group/refs/heads/main/security/tri-pointe-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Homebuilding
- Real Estate
- Residential Construction
- Mortgage
- Title And Escrow
- Insurance
- Smart Home
- Fortune 1000
- NYSE
- Public Company
---
