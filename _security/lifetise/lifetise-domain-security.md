---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coadjute.com
  spf: true
hosts:
- cert_expires: Sep 19 17:44:20 2026 GMT
  host: www.coadjute.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: marketing site (HubSpot)
  tls_version: TLSv1.3
- cert_expires: Dec 25 10:01:47 2026 GMT
  host: api.coadjute.com
  hsts: false
  http_status: 404
  https: true
  note: Answers a JSON error envelope to anonymous requests; no HSTS header returned.
  role: partner API gateway
  tls_version: TLSv1.3
- cert_expires: Sep 12 02:44:26 2026 GMT
  host: auth.coadjute.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: identity provider (Auth0 tenant)
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: app.coadjute.com
  hsts: false
  http_status: 200
  https: true
  role: customer web application
  tls_version: TLSv1.3
- cert_expires: Oct  4 08:22:32 2026 GMT
  host: status.coadjute.com
  hsts: true
  hsts_max_age: 259200
  https: true
  role: status page (Atlassian Statuspage)
  tls_version: TLSv1.3
- cert_expires: Dec 25 10:01:47 2026 GMT
  host: developer.coadjute.com
  hsts: false
  http_status: 502
  https: true
  note: TLS terminates cleanly but the origin is failing; certificate is shared with api.coadjute.com.
  role: retired developer portal
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lifetise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coadjute, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coadjute
provider_slug: lifetise
slug: lifetise-domain-security
source_filename: lifetise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus every Coadjute subdomain found\n  in the review probe log\nhosts:\n- host: www.coadjute.com\n  role: marketing site (HubSpot)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.coadjute.com\n  role: partner API gateway\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 10:01:47 2026 GMT\n  hsts: false\n  http_status: 404\n  note: Answers a JSON error envelope to anonymous requests; no HSTS header returned.\n- host: auth.coadjute.com\n  role: identity provider (Auth0 tenant)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: app.coadjute.com\n  role: customer web application\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n  http_status:\
  \ 200\n- host: status.coadjute.com\n  role: status page (Atlassian Statuspage)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 08:22:32 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: developer.coadjute.com\n  role: retired developer portal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 10:01:47 2026 GMT\n  hsts: false\n  http_status: 502\n  note: TLS terminates cleanly but the origin is failing; certificate is shared with\n    api.coadjute.com.\ndomains:\n- domain: coadjute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nobservations:\n- HSTS is inconsistent across the estate — present on the marketing site, the identity\n  tenant and the status page, absent on the API gateway and the customer application.\n- No CAA records are published, so certificate issuance is unconstrained.\n- DNSSEC is not enabled on coadjute.com.\n- DMARC is published at p=quarantine rather than p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifetise/refs/heads/main/security/lifetise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Transactions
- Conveyancing
- AML
- Compliance
- Distributed Ledger
- Estate Agents
- Mortgage
---
