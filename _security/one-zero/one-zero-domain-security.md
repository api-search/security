---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: onezerobank.com
  spf: true
hosts:
- cert_expires: Nov 13 01:59:20 2026 GMT
  host: www.onezerobank.com
  hsts: true
  hsts_header: max-age=15552000; includeSubDomains; preload
  hsts_max_age: 15552000
  https: true
  note: 'Origin is behind a Cloudflare managed challenge (HTTP 403, cf-mitigated: challenge) for non-browser clients; the HSTS header was read from that challenge response, which is served by the same edge.'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Zero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONE ZERO Digital Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ONE ZERO Digital Bank
provider_slug: one-zero
slug: one-zero-domain-security
source_filename: one-zero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onezerobank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 01:59:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_header: max-age=15552000; includeSubDomains; preload\n  note: 'Origin is behind a Cloudflare managed challenge (HTTP 403, cf-mitigated: challenge) for non-browser\n    clients; the HSTS header was read from that challenge response, which is served by the same edge.'\ndomains:\n- domain: onezerobank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: 'Every HTTP probe against www.onezerobank.com answers 403 with cf-mitigated: challenge. TLS, DNSSEC,\n  CAA, SPF and DMARC results are unaffected by that challenge; HTTP-body-dependent checks are not observable\n  from this vantage point.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-zero/refs/heads/main/security/one-zero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Financial-Services
- Fintech
- Digital Bank
- Open Banking
- Consumer Finance
- Israel
- Company
---
