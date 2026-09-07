---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: acqu.co
  note: _dmarc.acqu.co is a CNAME to acqu.co.hosted.dmarc-report.com, which returns no TXT record — a dangling DMARC delegation, so no DMARC policy is actually published. No DNSKEY (no DNSSEC) and no CAA record.
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: sellerfusion.io
  note: DNSSEC signed (2 DNSKEY records). No CAA. SPF v=spf1 include:_spf.google.com -all. No _dmarc TXT record.
  spf: true
hosts:
- cert_expires: Nov 26 16:48:19 2026 GMT
  host: www.acqu.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 16:44:04 2026 GMT
  host: sellerfusion.io
  hsts: false
  hsts_max_age: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 15:30:02 2026 GMT
  host: app.sellerfusion.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 14 19:17:30 2036 GMT
  host: api.sellerfusion.io
  hsts: false
  hsts_max_age: null
  https: false
  note: Resolves (CNAME demo-stby01.sellerfusion.io, 5.161.49.75) and serves a JSON API 404 envelope, but presents a SELF-SIGNED certificate for CN=scraper-proxy.easychamp.com — TLS validation fails for any client. No spec is served on it (/openapi.json, /swagger.json, /api-docs, /docs, /graphql all 404).
  tls_version: null
- cert_expires: null
  host: status.sellerfusion.io
  hsts: false
  hsts_max_age: null
  https: false
  note: Resolves (20.118.181.223) but presents the default 'Kubernetes Ingress Controller Fake Certificate' and returns an nginx 404 — an exposed ingress, not a status page.
  tls_version: null
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Acquco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acquco, probed live across 5 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Acquco
provider_slug: acquco
slug: acquco-domain-security
source_filename: acquco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (probe-domain-security.py), extended 2026-09-06\n  with the sellerfusion.io hosts, which are first-party Acquco surfaces but are not reachable from the\n  Website pointer the script walks\nhosts:\n- host: www.acqu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sellerfusion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 16:44:04 2026 GMT\n  hsts: false\n  hsts_max_age: null\n- host: app.sellerfusion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:30:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sellerfusion.io\n  https: false\n  tls_version: null\n  cert_expires: Apr 14 19:17:30 2036 GMT\n  hsts: false\n  hsts_max_age: null\n  note: Resolves (CNAME demo-stby01.sellerfusion.io, 5.161.49.75) and serves a JSON API 404 envelope,\n    but\
  \ presents a SELF-SIGNED certificate for CN=scraper-proxy.easychamp.com — TLS validation fails for\n    any client. No spec is served on it (/openapi.json, /swagger.json, /api-docs, /docs, /graphql all\n    404).\n- host: status.sellerfusion.io\n  https: false\n  tls_version: null\n  cert_expires: null\n  hsts: false\n  hsts_max_age: null\n  note: Resolves (20.118.181.223) but presents the default 'Kubernetes Ingress Controller Fake Certificate'\n    and returns an nginx 404 — an exposed ingress, not a status page.\ndomains:\n- domain: acqu.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  note: _dmarc.acqu.co is a CNAME to acqu.co.hosted.dmarc-report.com, which returns no TXT record — a\n    dangling DMARC delegation, so no DMARC policy is actually published. No DNSKEY (no DNSSEC) and no\n    CAA record.\n- domain: sellerfusion.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n  note: DNSSEC signed (2 DNSKEY records). No CAA. SPF v=spf1 include:_spf.google.com -all.\
  \ No _dmarc TXT\n    record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acquco/refs/heads/main/security/acquco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- E-Commerce
- Amazon
- Marketplaces
- Amazon FBA
- Aggregator
- Mergers And Acquisitions
- Seller Tools
- Analytics
- Retail
- SaaS
- New York
---
