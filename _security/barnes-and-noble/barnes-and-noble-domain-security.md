---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barnesandnoble.com
  spf: true
hosts:
- cert_expires: Aug 25 04:17:03 2026 GMT
  host: www.barnesandnoble.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: affiliate.barnesandnoble.com
  https: false
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: press.barnesandnoble.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barnes And Noble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barnes & Noble, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barnes & Noble
provider_slug: barnes-and-noble
slug: barnes-and-noble-domain-security
source_filename: barnes-and-noble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barnesandnoble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 04:17:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: affiliate.barnesandnoble.com\n  https: false\n- host: press.barnesandnoble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: barnesandnoble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barnes-and-noble/refs/heads/main/security/barnes-and-noble-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bookseller
- Books
- E-Commerce
- Education
- Retail
- Fortune 500
---
