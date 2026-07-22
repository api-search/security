---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@numer.ai"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: numer.ai
  spf: true
hosts:
- cert_expires: Sep 18 18:14:09 2026 GMT
  host: numer.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numerai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numerai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Numerai
provider_slug: numerai
slug: numerai-domain-security
source_filename: numerai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:14:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numer.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@numer.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numerai/refs/heads/main/security/numerai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Machine Learning
- Data Science
- Hedge Fund
- GraphQL
- Crypto
- Quantitative Finance
- Tournament
- API
---
