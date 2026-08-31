---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aarcorp.com
  spf: true
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trax.aero
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airinmar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: airvoyant.com
  note: DMARC rua/ruf report addresses point at trax.aero, confirming Airvoyant is operated out of the Trax organisation.
  spf: true
hosts:
- cert_expires: Nov  2 19:25:43 2026 GMT
  host: www.aarcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 19:25:43 2026 GMT
  host: www.trax.aero
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: aerostratsoftware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 10:26:45 2026 GMT
  host: shop.aarcorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: AAR PAARTS Store — the one live, anonymously reachable AAR API host (Adobe Commerce webapi at /rest/V1).
  tls_version: TLSv1.3
- cert_expires: Nov  2 19:25:43 2026 GMT
  host: api.aarcorp.com
  hsts: false
  https: true
  note: API gateway host. Answers a JSON 404 envelope on every path probed; no anonymous route found.
  tls_version: TLSv1.3
- cert_expires: Dec 15 13:43:43 2026 GMT
  host: www.airinmar.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: Airinmar subsidiary. Only AAR host observed negotiating TLS 1.2 rather than 1.3.
  tls_version: TLSv1.2
- cert_expires: Nov  9 17:39:21 2026 GMT
  host: www.airvoyant.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  note: Airvoyant subsidiary. HSTS max-age is 2,628,000s (~30 days), below the 1-year preload threshold.
  tls_version: TLSv1.3
- cert_expires: null
  host: myconnection.aarcorp.com
  hsts: null
  https: true
  note: Partner portal. TLS 1.3 handshake and HTTP/2 stream both complete (Let's Encrypt cert, CN=www.aarcorp.com, SAN covers myconnection.aarcorp.com) but the origin sends no response body within 15s. Probed once, not retried.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAR Corp, probed live across 8 host(s) and 4 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AAR Corp
provider_slug: aar
slug: aar-domain-security
source_filename: aar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every host in apis.yml (Website, humanURL, baseURL) plus the AAR-controlled\n  product and gateway hosts found during contract discovery on 2026-08-29\nhosts:\n- host: www.aarcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:25:43 2026 GMT\n  hsts: false\n- host: www.trax.aero\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:25:43 2026 GMT\n  hsts: false\n- host: aerostratsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: shop.aarcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 10:26:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: AAR PAARTS Store — the one live, anonymously reachable AAR API host (Adobe Commerce webapi at\n    /rest/V1).\n- host: api.aarcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 19:25:43\
  \ 2026 GMT\n  hsts: false\n  note: API gateway host. Answers a JSON 404 envelope on every path probed; no anonymous route found.\n- host: www.airinmar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 13:43:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  note: Airinmar subsidiary. Only AAR host observed negotiating TLS 1.2 rather than 1.3.\n- host: www.airvoyant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 17:39:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\n  note: Airvoyant subsidiary. HSTS max-age is 2,628,000s (~30 days), below the 1-year preload threshold.\n- host: myconnection.aarcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: null\n  hsts: null\n  note: Partner portal. TLS 1.3 handshake and HTTP/2 stream both complete (Let's Encrypt cert, CN=www.aarcorp.com,\n    SAN covers myconnection.aarcorp.com) but the origin sends no response body within 15s. Probed once,\n    not retried.\n\
  domains:\n- domain: aarcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: trax.aero\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: airinmar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: airvoyant.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC rua/ruf report addresses point at trax.aero, confirming Airvoyant is operated out of the\n    Trax organisation.\nsummary:\n  hosts_probed: 8\n  hsts_enabled: 4\n  hsts_missing:\n  - api.aarcorp.com\n  - www.aarcorp.com\n  - www.trax.aero\n  dnssec_enabled: 0\n  caa_present:\n  - trax.aero\n  note: No AAR registrable domain has DNSSEC. Only trax.aero\
  \ publishes CAA records. The corporate site\n    www.aarcorp.com and the api.aarcorp.com gateway both serve without HSTS, while every subsidiary host\n    has it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aar/refs/heads/main/security/aar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- MRO
- Aerospace
- Defense
- Parts Supply
- Maintenance
- Government
- Aviation Software
- Supply Chain
- E-Commerce
- Fortune 1000
---
