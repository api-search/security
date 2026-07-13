---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: barcodelookup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: upcitemdb.com
  spf: true
hosts:
- cert_expires: Oct  9 15:02:35 2026 GMT
  host: www.barcodelookup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 22 23:59:59 2026 GMT
  host: www.upcitemdb.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 29 03:31:22 2026 GMT
  host: www.ean-search.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barcode Scanners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barcode Scanners, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Barcode Scanners
provider_slug: barcode-scanners
slug: barcode-scanners-domain-security
source_filename: barcode-scanners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barcodelookup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:02:35 2026 GMT\n  hsts: null\n- host: www.upcitemdb.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 22 23:59:59 2026 GMT\n  hsts: false\n- host: www.ean-search.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 03:31:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barcodelookup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: upcitemdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barcode-scanners/refs/heads/main/security/barcode-scanners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Barcodes
- Inventory
- Product Lookup
- QR Codes
- Retail
- Scanning
- Supply Chain
---
