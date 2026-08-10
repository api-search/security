---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coolerx.com
  nameservers:
  - ns1-34.azure-dns.com
  - ns2-34.azure-dns.net
  - ns3-34.azure-dns.org
  - ns4-34.azure-dns.info
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  cert_issuer: DigiCert Inc / GeoTrust TLS RSA CA G1
  cert_subject: CN=www.coolerx.com
  host: www.coolerx.com
  hsts: null
  https: true
  notes: 'GET / returns 307 to https://coolerx.com/index.php and that redirect response carries no Strict-Transport-Security header. Application responses served from the origin (e.g. /index.php, /company/) do include "strict-transport-security: max-age=31536000; includeSubDomains; preload".'
  tls_version: TLSv1.3
- cert_expired: true
  cert_expires: Jun 10 23:59:59 2025 GMT
  cert_issuer: DigiCert, Inc. / GeoTrust Global TLS RSA4096 SHA256 2022 CA1
  cert_subject: CN=coolerx.com
  host: coolerx.com
  hsts: null
  https: false
  notes: The apex host serves a certificate that expired 2025-06-10, so every TLS client that validates the chain (curl, browsers, WebFetch) fails to connect. Observed consistently across the Azure Front Door addresses the apex resolves to (150.171.109.113 and 150.171.109.115). www.coolerx.com/ 307-redirects to https://coolerx.com/index.php, so the canonical homepage path terminates on the expired-certificate host. Probed 2026-08-09.
  tls_version: TLSv1.3
  verify_result: 10 (certificate has expired)
- dns_a: 13.67.211.230
  host: api.coolerx.com
  https: false
  notes: DNS A record resolves, but TCP connections to 443 and 80 time out. No service answered; treated as a private or firewalled partner endpoint, not a public API.
  reachable: false
- dns_a: 13.67.211.230
  host: portal.coolerx.com
  https: false
  notes: DNS A record resolves to the same address as api.coolerx.com; TCP connections to 443 and 80 time out.
  reachable: false
kind: domain-security
layout: security
method: probed
name: Cooler Screens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoolerX, probed live across 4 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CoolerX
provider_slug: cooler-screens
slug: cooler-screens-domain-security
source_filename: cooler-screens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coolerx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  cert_subject: CN=www.coolerx.com\n  cert_issuer: DigiCert Inc / GeoTrust TLS RSA CA G1\n  hsts: null\n  notes: >-\n    GET / returns 307 to https://coolerx.com/index.php and that redirect response\n    carries no Strict-Transport-Security header. Application responses served from\n    the origin (e.g. /index.php, /company/) do include\n    \"strict-transport-security: max-age=31536000; includeSubDomains; preload\".\n- host: coolerx.com\n  https: false\n  tls_version: TLSv1.3\n  cert_expires: Jun 10 23:59:59 2025 GMT\n  cert_subject: CN=coolerx.com\n  cert_issuer: DigiCert, Inc. / GeoTrust Global TLS RSA4096 SHA256 2022 CA1\n  cert_expired: true\n  verify_result: '10 (certificate has expired)'\n  hsts: null\n  notes: >-\n    The apex host serves a certificate\
  \ that expired 2025-06-10, so every TLS client\n    that validates the chain (curl, browsers, WebFetch) fails to connect. Observed\n    consistently across the Azure Front Door addresses the apex resolves to\n    (150.171.109.113 and 150.171.109.115). www.coolerx.com/ 307-redirects to\n    https://coolerx.com/index.php, so the canonical homepage path terminates on the\n    expired-certificate host. Probed 2026-08-09.\n- host: api.coolerx.com\n  https: false\n  reachable: false\n  dns_a: 13.67.211.230\n  notes: >-\n    DNS A record resolves, but TCP connections to 443 and 80 time out. No service\n    answered; treated as a private or firewalled partner endpoint, not a public API.\n- host: portal.coolerx.com\n  https: false\n  reachable: false\n  dns_a: 13.67.211.230\n  notes: >-\n    DNS A record resolves to the same address as api.coolerx.com; TCP connections to\n    443 and 80 time out.\ndomains:\n- domain: coolerx.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com\
  \ -all\n  dmarc: false\n  nameservers:\n  - ns1-34.azure-dns.com\n  - ns2-34.azure-dns.net\n  - ns3-34.azure-dns.org\n  - ns4-34.azure-dns.info\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooler-screens/refs/heads/main/security/cooler-screens-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Retail
- Retail Media
- Advertising
- Digital Signage
- In-Store Media
- Merchandising
- Artificial Intelligence
- Internet of Things
---
