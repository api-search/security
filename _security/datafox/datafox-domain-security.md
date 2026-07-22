---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: datafox.com
  nameservers:
  - ns1.p68.dns.oraclecloud.net
  - ns2.p68.dns.oraclecloud.net
  - ns3.p68.dns.oraclecloud.net
  - ns4.p68.dns.oraclecloud.net
  note: domain is under Oracle Cloud DNS with Oracle email-delivery SPF, confirming Oracle ownership post-acquisition. No CAA, no DMARC, no DNSSEC.
  spf: true
  spf_record: v=spf1 include:spf.oracleemaildelivery.com include:rp.oracleemaildelivery.com include:ap.rp.oracleemaildelivery.com include:eu.rp.oracleemaildelivery.com ~all
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
hosts:
- host: www.datafox.com
  hsts: false
  http: true
  http_status: 301
  https: false
  https_note: TLS handshake negotiates TLSv1.3 but the server returns a fatal internal error alert (SSL alert 80); HTTPS is effectively unusable.
  redirect_note: blanket redirect - every path, including /.well-known/* and /llms.txt, returns the same 301, so no discovery documents are actually served.
  redirects_to: https://www.oracle.com/corporate/acquisitions/datafox/
  server: AkamaiGHost
- address: 192.29.111.48
  host: api.datafox.com
  http: false
  https: false
  note: parked Oracle address; connection times out, no listening service.
  resolves: true
- address: 192.29.111.48
  host: app.datafox.com
  http: false
  https: false
  note: parked Oracle address; connection times out, no listening service.
  resolves: true
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datafox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataFox, probed live across 4 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DataFox
provider_slug: datafox
slug: datafox-domain-security
source_filename: datafox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: DataFox was acquired by Oracle and the standalone product is retired. The oracle.com\n  entries are the redirect target of www.datafox.com, not a DataFox-operated surface. The\n  datafox.com entries below were probed directly and record the legacy domain's posture.\nhosts:\n- host: www.datafox.com\n  https: false\n  https_note: TLS handshake negotiates TLSv1.3 but the server returns a fatal internal\n    error alert (SSL alert 80); HTTPS is effectively unusable.\n  http: true\n  http_status: 301\n  redirects_to: https://www.oracle.com/corporate/acquisitions/datafox/\n  redirect_note: blanket redirect - every path, including /.well-known/* and /llms.txt,\n    returns the same 301, so no discovery documents are actually served.\n  server: AkamaiGHost\n  hsts: false\n- host: api.datafox.com\n  https: false\n  http: false\n  resolves: true\n  address: 192.29.111.48\n  note:\
  \ parked Oracle address; connection times out, no listening service.\n- host: app.datafox.com\n  https: false\n  http: false\n  resolves: true\n  address: 192.29.111.48\n  note: parked Oracle address; connection times out, no listening service.\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datafox.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.oracleemaildelivery.com include:rp.oracleemaildelivery.com\n    include:ap.rp.oracleemaildelivery.com include:eu.rp.oracleemaildelivery.com ~all\n  dmarc: false\n  dmarc_policy: null\n  nameservers:\n  - ns1.p68.dns.oraclecloud.net\n  - ns2.p68.dns.oraclecloud.net\n  - ns3.p68.dns.oraclecloud.net\n  - ns4.p68.dns.oraclecloud.net\n  note: domain is under Oracle Cloud DNS with Oracle email-delivery SPF, confirming\n    Oracle ownership post-acquisition. No CAA, no DMARC, no DNSSEC.\n- domain: oracle.com\n\
  \  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafox/refs/heads/main/security/datafox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Company Data
- Sales Intelligence
- Data Enrichment
- Machine Learning
- Acquired
- Oracle
---
