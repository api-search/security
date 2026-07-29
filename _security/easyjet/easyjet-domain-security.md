---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_reporting: Proofpoint (dmarc_rua@emaildefense.proofpoint.com)
  dmarc_subdomain_policy: reject
  dnssec: false
  domain: easyjet.com
  note: 'Email authentication is at full enforcement: DMARC p=reject with sp=reject and forensic reporting. No DNSSEC signing and no CAA records are published, so certificate issuance is unconstrained at the DNS layer.'
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.easyjet.com
  hsts: false
  https: true
  note: Akamai-fronted public website. No Strict-Transport-Security header returned.
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.easyjet.com
  hsts: false
  https: true
  note: Production API hostname, CNAMEd to api.easyjet.com.edgekey.net. Reachable over TLS but returns HTTP 403 Akamai "Access Denied" on every path probed, including /openapi.json, /swagger.json, /graphql and the /.well-known/ discovery paths.
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: b2b.easyjet.com
  hsts: false
  https: true
  note: Business-to-business hostname, CNAMEd to b2b.easyjet.com.edgekey.net. TLS 1.3 terminates, then HTTP 403 Akamai "Access Denied" on every path probed.
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: brand.easyjet.com
  hsts: false
  https: true
  note: Production easyWidget / easyDom partner branding host. Serves Header.js and Footer.js anonymously with HTTP 200; partner-scoped widgets (Script.js, SignIn.js, Registration.js, VRPanel.js) return HTTP 200 with a zero-byte body for an unrecognised partner id. See components/easyjet-components.yml.
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: mobile.easyjet.com
  hsts: false
  https: true
  note: Mobile app backend host. HTTP 503 with an Akamai bot-defence script.
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:12:17 2026 GMT
  host: corporate.easyjet.com
  hsts: false
  https: true
  note: Investor relations site behind a Cloudflare managed challenge. /.well-known/security.txt answers HTTP 200 with the body "Invalid key" — a catch-all response, not an RFC 9116 security.txt.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Easyjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for easyJet, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: easyJet
provider_slug: easyjet
slug: easyjet-domain-security
source_filename: easyjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the easyJet API and partner\n  hosts discovered during contract discovery\nhosts:\n- host: www.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\n  note: Akamai-fronted public website. No Strict-Transport-Security header returned.\n- host: api.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    Production API hostname, CNAMEd to api.easyjet.com.edgekey.net. Reachable over\n    TLS but returns HTTP 403 Akamai \"Access Denied\" on every path probed, including\n    /openapi.json, /swagger.json, /graphql and the /.well-known/ discovery paths.\n- host: b2b.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    Business-to-business hostname, CNAMEd to b2b.easyjet.com.edgekey.net. TLS 1.3\n\
  \    terminates, then HTTP 403 Akamai \"Access Denied\" on every path probed.\n- host: brand.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n  note: >-\n    Production easyWidget / easyDom partner branding host. Serves Header.js and\n    Footer.js anonymously with HTTP 200; partner-scoped widgets (Script.js,\n    SignIn.js, Registration.js, VRPanel.js) return HTTP 200 with a zero-byte body\n    for an unrecognised partner id. See components/easyjet-components.yml.\n- host: mobile.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n  note: Mobile app backend host. HTTP 503 with an Akamai bot-defence script.\n- host: corporate.easyjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:12:17 2026 GMT\n  hsts: false\n  note: >-\n    Investor relations site behind a Cloudflare managed challenge.\n    /.well-known/security.txt answers HTTP 200 with the body\
  \ \"Invalid key\" — a\n    catch-all response, not an RFC 9116 security.txt.\ndomains:\n- domain: easyjet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_subdomain_policy: reject\n  dmarc_reporting: Proofpoint (dmarc_rua@emaildefense.proofpoint.com)\n  note: >-\n    Email authentication is at full enforcement: DMARC p=reject with sp=reject and\n    forensic reporting. No DNSSEC signing and no CAA records are published, so\n    certificate issuance is unconstrained at the DNS layer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easyjet/refs/heads/main/security/easyjet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Low Cost Carrier
- Europe
- Distribution
- Booking
- Ancillaries
- Partner Gated
---
