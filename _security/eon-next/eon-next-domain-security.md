---
description: 'Every E.ON Next host negotiates TLS 1.3 with a valid certificate, and the domain is registered on AWS Route 53. The weak spots are policy rather than transport: eonnext.com publishes no CAA record, no DNSSEC, and a DMARC record whose policy is p=none (monitor only, nothing quarantined or rejected). HSTS is served only by the Auth0-fronted identity host; the marketing/account site on S3 and both AWS API Gateway hosts send no Strict-Transport-Security header at all.'
domains:
- caa: []
  caa_note: No CAA record — any public CA may issue for this domain.
  dmarc: true
  dmarc_note: p=none is monitor-only, with no rua/ruf reporting address published, so spoofed mail is neither quarantined nor rejected.
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none
  dnssec: false
  domain: eonnext.com
  nameservers: AWS Route 53 (ns-1775.awsdns-29.co.uk, ns-218.awsdns-27.com, ns-628.awsdns-14.net, ns-1484.awsdns-57.org)
  spf: true
  spf_record: v=spf1 include:_spf.atlassian.net include:_spf.google.com include:sendgrid.net ip4:149.72.88.178 ~all
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.eonnext.com
  hsts: false
  http_status: 200
  https: true
  origin: AmazonS3
  other_headers:
  - 'x-frame-options: DENY'
  role: retail marketing and customer account website
  tls_version: TLSv1.3
- cert_expires: Oct  1 05:32:37 2026 GMT
  cert_issuer: Let's Encrypt (CN=YE1)
  host: auth.eonnext.com
  hsts: true
  hsts_header: max-age=31536000; includeSubDomains
  hsts_max_age: 31536000
  http_status: 302
  https: true
  origin: cloudflare
  other_headers:
  - 'x-content-type-options: nosniff'
  role: E.ON CIAM authorization server (Auth0 tenant eon-ciam, application eon-next-uk)
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: api.eonnext.com
  hsts: false
  http_status: 403
  http_status_note: '{"message":"Missing Authentication Token"} on every path probed.'
  https: true
  role: undocumented AWS API Gateway deployment
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M04
  host: data.eonnext.com
  hsts: false
  http_status: 403
  https: true
  role: second AWS API Gateway deployment; not an open-data portal
  tls_version: TLSv1.3
- cert_expires: Oct 19 05:48:16 2026 GMT
  cert_issuer: Google Trust Services (CN=WR3)
  host: community.eonnext.com
  hsts: false
  http_status: 200
  https: true
  origin: nginx
  role: customer community forum (Anubis proof-of-work anti-scraping in front)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eon Next Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for E.ON Next, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: E.ON Next
provider_slug: eon-next
slug: eon-next-domain-security
source_filename: eon-next-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the apis.yml hosts\n  (0-working/probe-domain-security.py), extended by hand on the same date with\n  `curl -sI`, `openssl s_client` and `dig` for the four hosts the script does not\n  reach from apis.yml alone — api.eonnext.com, data.eonnext.com,\n  auth.eonnext.com and community.eonnext.com. Observed header values are recorded\n  verbatim; absence of a record is real data, not a gap in the probe.\ndescription: >-\n  Every E.ON Next host negotiates TLS 1.3 with a valid certificate, and the\n  domain is registered on AWS Route 53. The weak spots are policy rather than\n  transport: eonnext.com publishes no CAA record, no DNSSEC, and a DMARC record\n  whose policy is p=none (monitor only, nothing quarantined or rejected). HSTS is\n  served only by the Auth0-fronted identity host; the marketing/account site on\n  S3 and both AWS API Gateway hosts send no Strict-Transport-Security header at\n  all.\n\
  hosts:\n- host: www.eonnext.com\n  role: retail marketing and customer account website\n  https: true\n  http_status: 200\n  origin: AmazonS3\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n  other_headers:\n  - 'x-frame-options: DENY'\n- host: auth.eonnext.com\n  role: E.ON CIAM authorization server (Auth0 tenant eon-ciam, application eon-next-uk)\n  https: true\n  http_status: 302\n  origin: cloudflare\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (CN=YE1)\n  cert_expires: Oct  1 05:32:37 2026 GMT\n  hsts: true\n  hsts_header: 'max-age=31536000; includeSubDomains'\n  hsts_max_age: 31536000\n  other_headers:\n  - 'x-content-type-options: nosniff'\n- host: api.eonnext.com\n  role: undocumented AWS API Gateway deployment\n  https: true\n  http_status: 403\n  http_status_note: '{\"message\":\"Missing Authentication Token\"} on every path probed.'\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M01\n  cert_expires: Jan 24 23:59:59 2027 GMT\n\
  \  hsts: false\n- host: data.eonnext.com\n  role: second AWS API Gateway deployment; not an open-data portal\n  https: true\n  http_status: 403\n  tls_version: TLSv1.3\n  cert_issuer: Amazon RSA 2048 M04\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: community.eonnext.com\n  role: customer community forum (Anubis proof-of-work anti-scraping in front)\n  https: true\n  http_status: 200\n  origin: nginx\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (CN=WR3)\n  cert_expires: Oct 19 05:48:16 2026 GMT\n  hsts: false\ndomains:\n- domain: eonnext.com\n  nameservers: AWS Route 53 (ns-1775.awsdns-29.co.uk, ns-218.awsdns-27.com, ns-628.awsdns-14.net, ns-1484.awsdns-57.org)\n  dnssec: false\n  caa: []\n  caa_note: No CAA record — any public CA may issue for this domain.\n  spf: true\n  spf_record: 'v=spf1 include:_spf.atlassian.net include:_spf.google.com include:sendgrid.net ip4:149.72.88.178 ~all'\n  dmarc: true\n  dmarc_record: 'v=DMARC1; p=none'\n  dmarc_policy:\
  \ none\n  dmarc_note: >-\n    p=none is monitor-only, with no rua/ruf reporting address published, so\n    spoofed mail is neither quarantined nor rejected.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eon-next/refs/heads/main/security/eon-next-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Energy Retail
- Kraken
- Solar
- EV Charging
- Identity
---
