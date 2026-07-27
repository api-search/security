---
api_specs:
- filename: offerpad-wordpress-wp-v2-openapi.yml
  format: yaml
  label: Offerpad WordPress REST API
  slug: offerpad-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/openapi/offerpad-wordpress-wp-v2-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: offerpad.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Oct 19 18:02:32 2026 GMT
  host: www.offerpad.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 23:45:10 2026 GMT
  host: connect.offerpad.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Offerpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offerpad, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Offerpad
provider_slug: offerpad
slug: offerpad-domain-security
source_filename: offerpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.offerpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 18:02:32 2026 GMT\n  hsts: false\n- host: connect.offerpad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:45:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: offerpad.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\
  \n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/offerpad/refs/heads/main/security/offerpad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United States
- iBuyer
- PropTech
- Property Listings
- Brokerage
- MLS
- Cash Offer
- Renovation
- Home Buying
---
