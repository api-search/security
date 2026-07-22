---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-reports@ridecell.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ridecell.com
  spf: true
hosts:
- cert_expires: Oct  8 03:35:06 2026 GMT
  host: ridecell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ridecell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ridecell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ridecell
provider_slug: ridecell
slug: ridecell-domain-security
source_filename: ridecell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridecell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:35:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ridecell.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-reports@ridecell.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ridecell/refs/heads/main/security/ridecell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Saas
- Fleet Management
- Mobility
- Automotive
- Artificial Intelligence
- Asset Intelligence
- Automation
---
