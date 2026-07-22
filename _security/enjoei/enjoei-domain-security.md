---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enjoei.com.br
  spf: true
hosts:
- cert_expires: Aug 30 15:45:31 2026 GMT
  host: www.enjoei.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enjoei Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enjoei, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enjoei
provider_slug: enjoei
slug: enjoei-domain-security
source_filename: enjoei-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enjoei.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:45:31 2026 GMT\n  hsts: false\ndomains:\n- domain: enjoei.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enjoei/refs/heads/main/security/enjoei-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Marketplace
- E-commerce
- Resale
- Secondhand
- Fashion
- Brazil
---
