---
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_pct: 1
  dmarc_policy: quarantine
  dmarc_rua: mailto:mailauth-reports@hike.in
  dmarc_subdomain_policy: reject
  dnskey: []
  dnssec: false
  domain: hike.in
  ds: []
  mx: google-workspace
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:amazonses.com ~all
hosts:
- cert_expired: true
  cert_expires: '2026-07-01T07:18:19Z'
  cert_issuer: C=US, ST=Arizona, L=Scottsdale, O=GoDaddy.com, Inc., CN=Go Daddy Secure Certificate Authority - G2
  cert_not_before: '2025-06-18T05:34:31Z'
  cert_subject: CN=*.hike.in
  host: hike.in
  hsts: false
  http_note: origin returns a Google Front End "502 Server Error" page for every path
  http_status: 502
  https: true
  tls_verify: 'failed: certificate has expired (openssl verify code 10)'
  tls_version: TLSv1.3
- cert_expired: true
  dns: CNAME hike.in
  host: www.hike.in
  hsts: false
  http_status: 502
  https: true
- cert_expired: true
  dns: A 34.54.124.161
  host: ai.hike.in
  hsts: false
  http_status: 502
  https: true
- dns: A 52.0.16.118
  host: blog.hike.in
  http_note: connection timed out after 15s
  http_status: null
  https: false
- dns: A 10.20.0.23
  host: docs.hike.in
  http_note: public DNS answers with an RFC 1918 private address; the record survives in the zone but points at an internal host that is not routable from the internet
  https: false
- dns: A 10.25.0.38
  host: dev.hike.in
  http_note: public DNS answers with an RFC 1918 private address; not routable from the internet
  https: false
kind: domain-security
layout: security
method: probed
name: Hike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hike, probed live across 6 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hike
provider_slug: hike
slug: hike-domain-security
source_filename: hike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live TLS + DNS probe of hike.in (openssl s_client, curl, dig @8.8.8.8)\nnote: >-\n  Hike Private Limited wound down completely in September 2025 after India's Promotion\n  and Regulation of Online Gaming Act, 2025. The DNS zone for hike.in is still published\n  (Route 53), but the origin behind it is gone: every HTTPS request returns a Google\n  Front End 502 and the wildcard certificate expired on 2026-07-01. Every developer-facing\n  subdomain that ever appeared in Certificate Transparency (platform.hike.in, hub.hike.in,\n  im.hike.in, faq.hike.in, support.hike.in, press.hike.in, shop.hike.in, discourse.hike.in)\n  is now NXDOMAIN. This record captures the residual posture of a decommissioned estate,\n  not a running service.\nhosts:\n- host: hike.in\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=*.hike.in\n  cert_issuer: 'C=US, ST=Arizona, L=Scottsdale, O=GoDaddy.com, Inc., CN=Go Daddy Secure Certificate Authority\
  \ - G2'\n  cert_not_before: '2025-06-18T05:34:31Z'\n  cert_expires: '2026-07-01T07:18:19Z'\n  cert_expired: true\n  tls_verify: 'failed: certificate has expired (openssl verify code 10)'\n  http_status: 502\n  http_note: origin returns a Google Front End \"502 Server Error\" page for every path\n  hsts: false\n- host: www.hike.in\n  dns: CNAME hike.in\n  https: true\n  cert_expired: true\n  http_status: 502\n  hsts: false\n- host: ai.hike.in\n  dns: A 34.54.124.161\n  https: true\n  cert_expired: true\n  http_status: 502\n  hsts: false\n- host: blog.hike.in\n  dns: A 52.0.16.118\n  https: false\n  http_status: null\n  http_note: connection timed out after 15s\n- host: docs.hike.in\n  dns: A 10.20.0.23\n  https: false\n  http_note: >-\n    public DNS answers with an RFC 1918 private address; the record survives in the zone\n    but points at an internal host that is not routable from the internet\n- host: dev.hike.in\n  dns: A 10.25.0.38\n  https: false\n  http_note: >-\n    public DNS\
  \ answers with an RFC 1918 private address; not routable from the internet\nnxdomain_hosts:\n- platform.hike.in\n- hub.hike.in\n- im.hike.in\n- faq.hike.in\n- support.hike.in\n- press.hike.in\n- shop.hike.in\n- discourse.hike.in\n- api.hike.in\n- developer.hike.in\ndomains:\n- domain: hike.in\n  dnssec: false\n  dnskey: []\n  ds: []\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:amazonses.com ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_subdomain_policy: reject\n  dmarc_pct: 1\n  dmarc_rua: mailto:mailauth-reports@hike.in\n  mx: google-workspace\nx-evidence:\n- {probe: 'openssl s_client -connect hike.in:443', result: 'verify error:num=10:certificate has expired'}\n- {probe: 'curl -k https://hike.in/', result: 'HTTP 502'}\n- {probe: 'dig DNSKEY hike.in', result: empty}\n- {probe: 'dig CAA hike.in', result: '0 issuewild \"godaddy.com\"'}\n- {probe: 'dig TXT _dmarc.hike.in', result: 'v=DMARC1; p=quarantine; sp=reject'}\n\
  - {probe: 'crt.sh %.hike.in', result: '33 historical names; every developer subdomain now NXDOMAIN'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hike/refs/heads/main/security/hike-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Messaging
- Social
- Gaming
- Mobile
- Consumer
- Web3
- India
- Defunct
---
