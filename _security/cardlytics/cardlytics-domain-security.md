---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "trust-provider.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cardlytics.com
  spf: true
hosts:
- cert_expires: Aug 28 21:59:33 2026 GMT
  host: www.cardlytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cardlytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardlytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cardlytics
provider_slug: cardlytics
slug: cardlytics-domain-security
source_filename: cardlytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cardlytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:59:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cardlytics.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardlytics/refs/heads/main/security/cardlytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Commerce Media
- Card-Linked Offers
- Purchase Intelligence
- Financial Services
- Loyalty and Rewards
- Marketing
---
