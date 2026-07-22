---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: listia.com
  spf: true
hosts:
- cert_expires: Oct 11 17:03:20 2026 GMT
  host: www.listia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Listia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Listia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Listia
provider_slug: listia
slug: listia-domain-security
source_filename: listia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.listia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 17:03:20 2026 GMT\n  hsts: false\ndomains:\n- domain: listia.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/listia/refs/heads/main/security/listia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplace
- Ecommerce
- Peer to Peer
- Auctions
- Reuse
- Secondhand
- Virtual Currency
- Consumer
- Mobile Apps
---
