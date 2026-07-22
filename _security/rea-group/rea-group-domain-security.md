---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@rea-group.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rea-group.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:pt-systems-support@rea-group.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: proptrack.com.au
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.rea-group.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:33:34 2026 GMT
  host: developer.proptrack.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:37:58 2026 GMT
  host: data.proptrack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rea Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REA Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: REA Group
provider_slug: rea-group
slug: rea-group-domain-security
source_filename: rea-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rea-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.proptrack.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.proptrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:37:58 2026 GMT\n  hsts: null\ndomains:\n- domain: rea-group.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@rea-group.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: proptrack.com.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:pt-systems-support@rea-group.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/security/rea-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Property Data
- Valuations
- Market Insights
- Listings
- PropTech
- Australia
---
