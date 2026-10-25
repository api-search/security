---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hmccapital.com.au
  spf: true
hosts:
- cert_expires: Jan  8 04:55:40 2027 GMT
  host: hmccapital.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homeco Daily Needs Reit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeCo Daily Needs REIT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HomeCo Daily Needs REIT
provider_slug: homeco-daily-needs-reit
slug: homeco-daily-needs-reit-domain-security
source_filename: homeco-daily-needs-reit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hmccapital.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 04:55:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hmccapital.com.au\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeco-daily-needs-reit/refs/heads/main/security/homeco-daily-needs-reit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- REIT
- Retail Property
- Australia
- ASX Listed
- Investment Trust
---
