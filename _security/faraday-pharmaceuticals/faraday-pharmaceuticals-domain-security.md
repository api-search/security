---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  dnssec: false
  domain: faradaypharma.com
  mx: true
  mx_hosts:
  - faradaypharma.in.tmes.trendmicro.com
  nameservers:
  - ns01.squarespacedns.com
  - ns02.squarespacedns.com
  - ns03.squarespacedns.com
  - ns04.squarespacedns.com
  - dns1.p03.nsone.net
  - dns2.p03.nsone.net
  - dns3.p03.nsone.net
  - dns4.p03.nsone.net
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:spf.tmes.trendmicro.com -all
hosts:
- cert_expires: Oct  6 04:25:41 2026 GMT
  cert_issuer: Let's Encrypt
  host: www.faradaypharma.com
  hsts: true
  hsts_max_age: 15552000
  http_status: 404
  https: true
  server: Squarespace
  serving_content: false
  tls_version: TLSv1.3
- cert_expires: Oct 16 19:15:41 2026 GMT
  cert_issuer: Let's Encrypt
  host: faradaypharma.com
  http_status: 404
  https: true
  server: Squarespace
  serving_content: false
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Faraday Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faraday Pharmaceuticals, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Faraday Pharmaceuticals
provider_slug: faraday-pharmaceuticals
slug: faraday-pharmaceuticals-domain-security
source_filename: faraday-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS + TLS probe of faradaypharma.com (dig, openssl s_client, HTTP HEAD)\nnote: >-\n  Faraday Pharmaceuticals ceased operations in February 2026. The corporate domain still\n  resolves and still carries live mail-authentication records, but the website itself is no\n  longer served — every path returns HTTP 404 with the Squarespace \"Website Expired\" page.\n  These readings describe a parked/wound-down domain, not an operating API surface.\nhosts:\n- host: www.faradaypharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt\"\n  cert_expires: 'Oct  6 04:25:41 2026 GMT'\n  hsts: true\n  hsts_max_age: 15552000\n  http_status: 404\n  server: Squarespace\n  serving_content: false\n- host: faradaypharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: \"Let's Encrypt\"\n  cert_expires: 'Oct 16 19:15:41 2026 GMT'\n  http_status: 404\n  server: Squarespace\n  serving_content: false\ndomains:\n\
  - domain: faradaypharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com include:spf.tmes.trendmicro.com -all'\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  mx: true\n  mx_hosts:\n  - faradaypharma.in.tmes.trendmicro.com\n  nameservers:\n  - ns01.squarespacedns.com\n  - ns02.squarespacedns.com\n  - ns03.squarespacedns.com\n  - ns04.squarespacedns.com\n  - dns1.p03.nsone.net\n  - dns2.p03.nsone.net\n  - dns3.p03.nsone.net\n  - dns4.p03.nsone.net\nx-evidence:\n  fetched: '2026-08-04'\n  dns_queries: [A, NS, MX, TXT, CAA, DNSKEY, _dmarc TXT]\n  tls_probe: openssl s_client TLSv1.3 handshake, verify return code 0 (ok)\n  http_probe: 'HEAD https://www.faradaypharma.com/ -> HTTP/2 404, server: Squarespace'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faraday-pharmaceuticals/refs/heads/main/security/faraday-pharmaceuticals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Life Sciences
- Clinical Trials
- Clinical Stage
- Cardiology
- Drug Development
- Defunct
---
