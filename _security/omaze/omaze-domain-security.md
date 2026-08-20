---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: omaze.com
  spf: true
- caa:
  - 0 issuewild "awstrust.com"
  - 128 issue "letsencrypt.org"
  - 128 issue "www.digicert.com"
  - 128 issue "www.globalsign.com"
  - 128 issuewild "letsencrypt.org"
  - 128 issuewild "www.digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: omaze.co.uk
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: www.omaze.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 20:08:32 2026 GMT
  host: omaze.co.uk
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 19:12:34 2026 GMT
  host: omaze.de
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omaze, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Omaze
provider_slug: omaze
slug: omaze-domain-security
source_filename: omaze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omaze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: false\n- host: omaze.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 20:08:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: omaze.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 19:12:34 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: omaze.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: omaze.co.uk\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"www.digicert.com\"\n  - 128 issue \"www.globalsign.com\"\n  - 128 issuewild \"letsencrypt.org\"\n  - 128 issuewild \"www.digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omaze/refs/heads/main/security/omaze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Charity
- Fundraising
- Non-Profit
- Prize Draws
- Sweepstakes
- E-Commerce
- Agentic Commerce
- Universal Commerce Protocol
- MCP
- Shopify
- United Kingdom
- Germany
---
