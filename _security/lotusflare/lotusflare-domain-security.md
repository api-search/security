---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lotusflare.com
  spf: true
hosts:
- cert_expires: Oct 17 16:40:49 2026 GMT
  host: lotusflare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lotusflare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LotusFlare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LotusFlare
provider_slug: lotusflare
slug: lotusflare-domain-security
source_filename: lotusflare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lotusflare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:40:49 2026 GMT\n  hsts: false\ndomains:\n- domain: lotusflare.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lotusflare/refs/heads/main/security/lotusflare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Telecommunications
- BSS
- Digital Commerce
- Monetization
- Cloud
- SaaS
- eSIM
---
