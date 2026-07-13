---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "globalsign.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flipkart.com
  spf: true
hosts:
- cert_expires: Aug 29 13:30:06 2026 GMT
  host: seller.flipkart.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flipkart Marketplace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flipkart Marketplace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Flipkart Marketplace
provider_slug: flipkart-marketplace
slug: flipkart-marketplace-domain-security
source_filename: flipkart-marketplace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seller.flipkart.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 29 13:30:06 2026 GMT\n  hsts: false\ndomains:\n- domain: flipkart.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flipkart-marketplace/refs/heads/main/security/flipkart-marketplace-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Shopping
- Public APIs
---
