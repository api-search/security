---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_rua: mailto:dmarc@choicehotels.com
  dnssec: false
  domain: choicehotels.com
  mta_sts: false
  spf: true
  spf_record: v=spf1 include:_spf.choicehotels.com ~all
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: choicehotelsdevelopment.com
  mta_sts: false
  spf: true
  spf_record: v=spf1 include:_spf.sparkpostmail.com ip4:52.40.103.197 ~all
hosts:
- cert_expires: Nov  3 23:59:59 2026 GMT
  cert_hostname_match: true
  cert_subject: CN=www.choicehotels.com, O=CHOICE HOTELS INTERNATIONAL, INC.
  host: www.choicehotels.com
  hsts: null
  hsts_max_age: null
  http_status: 0
  https: true
  note: Akamai edge terminates HTTP/2 with INTERNAL_ERROR and resets HTTP/1.1 for non-browser clients, so response headers (including any HSTS) cannot be read by tooling. Bot management, not an outage.
  role: website
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  cert_finding: TLS hostname mismatch — the certificate presented for api.choicehotels.com is the TIBCO Mashery certificate (CN=mashery.com, SANs cover *.mashery.com only, no choicehotels.com SAN). Standard verifying clients fail the handshake with "no alternative certificate subject name matches target host name". Verified 2026-07-28; certificate issued 2026-03-23.
  cert_hostname_match: false
  cert_subject: CN=mashery.com
  host: api.choicehotels.com
  hsts: false
  http_note: 'With certificate verification disabled the gateway answers HTTP/1.1 596 with Server: Mashery Proxy and X-Mashery-Error-Code: ERR_596_SERVICE_NOT_FOUND on every probed path — a live gateway with no publicly mapped service.'
  http_status: 596
  https: true
  role: api-gateway
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  cert_finding: Same Mashery certificate and same hostname mismatch as api.choicehotels.com.
  cert_hostname_match: false
  cert_subject: CN=mashery.com
  host: developer.choicehotels.com
  hsts: false
  http_status: 404
  https: true
  role: unprovisioned-developer-portal
  tls_version: TLSv1.3
- cert_expires: Oct 25 04:12:18 2026 GMT
  cert_hostname_match: true
  cert_subject: CN=connect.choicehotels.com
  host: connect.choicehotels.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 302
  https: true
  role: franchisee-login
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:02:34 2026 GMT
  cert_hostname_match: true
  cert_subject: CN=media.choicehotels.com
  host: media.choicehotels.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
  note: Only host in the estate still negotiating TLS 1.2 rather than TLS 1.3.
  role: press-room
  tls_version: TLSv1.2
- cert_expires: Oct  2 12:17:34 2026 GMT
  cert_hostname_match: true
  cert_subject: CN=investor.choicehotels.com
  host: investor.choicehotels.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 403
  https: true
  note: 'Cloudflare challenge (cf-mitigated: challenge) on the document root for automated clients.'
  role: investor-relations
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:40:38 2026 GMT
  cert_hostname_match: true
  cert_subject: CN=www.choicehotelsdevelopment.com
  host: www.choicehotelsdevelopment.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  http_status: 200
  https: true
  role: franchise-development-site
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Choice Hotels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Choice Hotels, probed live across 7 host(s) and 2 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Choice Hotels
provider_slug: choice-hotels
slug: choice-hotels-domain-security
source_filename: choice-hotels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (no OpenAPI servers[] exist for\n  this provider)\nhosts:\n- host: www.choicehotels.com\n  role: website\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=www.choicehotels.com, O=CHOICE HOTELS INTERNATIONAL, INC.\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  cert_hostname_match: true\n  hsts: null\n  hsts_max_age: null\n  http_status: 000\n  note: Akamai edge terminates HTTP/2 with INTERNAL_ERROR and resets HTTP/1.1 for non-browser\n    clients, so response headers (including any HSTS) cannot be read by tooling. Bot\n    management, not an outage.\n- host: api.choicehotels.com\n  role: api-gateway\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=mashery.com\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  cert_hostname_match: false\n  cert_finding: TLS hostname mismatch — the certificate presented for api.choicehotels.com\n    is the TIBCO Mashery certificate (CN=mashery.com,\
  \ SANs cover *.mashery.com only,\n    no choicehotels.com SAN). Standard verifying clients fail the handshake with \"no\n    alternative certificate subject name matches target host name\". Verified 2026-07-28;\n    certificate issued 2026-03-23.\n  hsts: false\n  http_status: 596\n  http_note: 'With certificate verification disabled the gateway answers HTTP/1.1 596\n    with Server: Mashery Proxy and X-Mashery-Error-Code: ERR_596_SERVICE_NOT_FOUND\n    on every probed path — a live gateway with no publicly mapped service.'\n- host: developer.choicehotels.com\n  role: unprovisioned-developer-portal\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=mashery.com\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  cert_hostname_match: false\n  cert_finding: Same Mashery certificate and same hostname mismatch as api.choicehotels.com.\n  hsts: false\n  http_status: 404\n- host: connect.choicehotels.com\n  role: franchisee-login\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=connect.choicehotels.com\n\
  \  cert_expires: Oct 25 04:12:18 2026 GMT\n  cert_hostname_match: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  http_status: 302\n- host: media.choicehotels.com\n  role: press-room\n  https: true\n  tls_version: TLSv1.2\n  cert_subject: CN=media.choicehotels.com\n  cert_expires: Oct  4 08:02:34 2026 GMT\n  cert_hostname_match: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  http_status: 200\n  note: Only host in the estate still negotiating TLS 1.2 rather than TLS 1.3.\n- host: investor.choicehotels.com\n  role: investor-relations\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=investor.choicehotels.com\n  cert_expires: Oct  2 12:17:34 2026 GMT\n  cert_hostname_match: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 403\n  note: 'Cloudflare challenge (cf-mitigated: challenge) on the document root for automated\n    clients.'\n- host: www.choicehotelsdevelopment.com\n\
  \  role: franchise-development-site\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=www.choicehotelsdevelopment.com\n  cert_expires: Sep 29 10:40:38 2026 GMT\n  cert_hostname_match: true\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  http_status: 200\ndomains:\n- domain: choicehotels.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.choicehotels.com ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_rua: mailto:dmarc@choicehotels.com\n  mta_sts: false\n- domain: choicehotelsdevelopment.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.sparkpostmail.com ip4:52.40.103.197 ~all\n  dmarc: true\n  dmarc_policy: none\n  mta_sts: false\nfindings:\n- id: api-host-cert-mismatch\n  severity: notable\n  summary: api.choicehotels.com and developer.choicehotels.com both present the TIBCO\n    Mashery wildcard certificate (CN=mashery.com) with no choicehotels.com SAN, so\n    HTTPS to the API gateway\
  \ fails certificate verification in any standard client.\n- id: no-caa\n  severity: informational\n  summary: Neither registrable domain publishes CAA records, so no certificate authority\n    is constrained from issuing for these names.\n- id: no-dnssec\n  severity: informational\n  summary: Neither registrable domain is DNSSEC-signed.\n- id: dmarc-monitor-only\n  severity: informational\n  summary: Both domains publish DMARC at p=none (monitor only) — no quarantine or\n    reject enforcement.\n- id: no-hsts-on-api-hosts\n  severity: informational\n  summary: The Mashery-fronted api. and developer. hosts return no Strict-Transport-Security\n    header; every non-Mashery host in the estate does send HSTS with includeSubDomains.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/choice-hotels/refs/heads/main/security/choice-hotels-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United States
- Hospitality
- Hotels
- Booking
- Reservations
- Distribution
- Franchising
- Loyalty
---
