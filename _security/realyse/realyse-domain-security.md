---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security-reports-aaaap4ofqt5foklwk37dle4k3i@realyseteam.slack.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realyse.com
  spf: true
hosts:
- cert_expires: Sep 29 10:03:12 2026 GMT
  host: www.realyse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Realyse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REalyse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: REalyse
provider_slug: realyse
slug: realyse-domain-security
source_filename: realyse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realyse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: realyse.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security-reports-aaaap4ofqt5foklwk37dle4k3i@realyseteam.slack.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realyse/refs/heads/main/security/realyse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Property
- Real Estate
- Data
- Analytics
- Geospatial
- Market Intelligence
- Residential
- United Kingdom
- PropTech
---
