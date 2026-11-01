---
description: ''
domains:
- caa:
  - 0 iodef "mailto:ie@pollyex.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pollyex.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: pollyex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pollyex Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polly
provider_slug: pollyex-com
slug: pollyex-com-domain-security
source_filename: pollyex-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pollyex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pollyex.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ie@pollyex.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/pollyex-com/security/pollyex-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- CapitalMarkets
- AI
- Mortgage
---
