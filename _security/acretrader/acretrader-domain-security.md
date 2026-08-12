---
description: AcreTrader publishes no public developer API and declares no baseURL or OpenAPI servers[], so the corporate host acretrader.com was probed directly, together with api.acretrader.com — a live first-party backend host discovered in this round via a first-party RSS link on the AcreTrader homepage. Absence of a record (CAA, DNSSEC, HSTS) is valid, recorded data for an investment marketing site, not a gap in a developer API surface.
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: mailto:admin@acretrader.com
  dnssec: false
  domain: acretrader.com
  nameservers:
  - ns-cloud-b1.googledomains.com
  - ns-cloud-b2.googledomains.com
  - ns-cloud-b3.googledomains.com
  - ns-cloud-b4.googledomains.com
  note: A wildcard A record answers for every acretrader.com subdomain (34.111.30.82) — a randomly generated subdomain resolves and returns the same response — so the existence of developer./docs./status./app.acretrader.com is a DNS artifact, not evidence of those services. That wildcard target answers with a Kubernetes API server 403 ('system:anonymous cannot get path "/"'), which is an exposure worth reporting to AcreTrader. api.acretrader.com is a distinct address (34.111.83.6) and is a real service.
  spf: true
  spf_record: v=spf1 mx include:_spf.google.com ip4:152.70.150.118 ip4:129.213.11.79 include:spf.protection.outlook.com include:sendgrid.net -all
hosts:
- cert_expires: Nov  1 23:55:04 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  csp: false
  host: acretrader.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Served from Google Cloud (UploadServer signature). Markup is pre-rendered HTML; www.acretrader.com redirects to the apex host.
  server: UploadServer
  tls_version: TLSv1.3
- cert_expires: Nov  7 11:13:56 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  csp: false
  host: api.acretrader.com
  hsts: false
  hsts_max_age: null
  http_status_root: 404
  https: true
  note: Google Cloud HTTPS load balancer with path-based routing ("service rules for the path non-existent" on unmatched paths). /healthz returns 200 "alive". No /.well-known/ document, no OpenAPI/Swagger and no GraphQL surface is served — see well-known/acretrader-well-known.yml for the full probe table.
  server: null
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acretrader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acretrader, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acretrader
provider_slug: acretrader
slug: acretrader-domain-security
source_filename: acretrader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of acretrader.com and api.acretrader.com\ndescription: >-\n  AcreTrader publishes no public developer API and declares no baseURL or OpenAPI\n  servers[], so the corporate host acretrader.com was probed directly, together with\n  api.acretrader.com — a live first-party backend host discovered in this round via a\n  first-party RSS link on the AcreTrader homepage. Absence of a record (CAA, DNSSEC,\n  HSTS) is valid, recorded data for an investment marketing site, not a gap in a\n  developer API surface.\nhosts:\n- host: acretrader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Nov  1 23:55:04 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  csp: false\n  server: UploadServer\n  note: >-\n    Served from Google Cloud (UploadServer signature). Markup is pre-rendered HTML;\n    www.acretrader.com redirects to the apex host.\n- host: api.acretrader.com\n\
  \  https: true\n  http_status_root: 404\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Nov  7 11:13:56 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  csp: false\n  server: null\n  note: >-\n    Google Cloud HTTPS load balancer with path-based routing (\"service rules for the\n    path non-existent\" on unmatched paths). /healthz returns 200 \"alive\". No\n    /.well-known/ document, no OpenAPI/Swagger and no GraphQL surface is served — see\n    well-known/acretrader-well-known.yml for the full probe table.\ndomains:\n- domain: acretrader.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: >-\n    v=spf1 mx include:_spf.google.com ip4:152.70.150.118 ip4:129.213.11.79\n    include:spf.protection.outlook.com include:sendgrid.net -all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: mailto:admin@acretrader.com\n  nameservers:\n  - ns-cloud-b1.googledomains.com\n  - ns-cloud-b2.googledomains.com\n  - ns-cloud-b3.googledomains.com\n  -\
  \ ns-cloud-b4.googledomains.com\n  note: >-\n    A wildcard A record answers for every acretrader.com subdomain (34.111.30.82) — a\n    randomly generated subdomain resolves and returns the same response — so the\n    existence of developer./docs./status./app.acretrader.com is a DNS artifact, not\n    evidence of those services. That wildcard target answers with a Kubernetes API\n    server 403 ('system:anonymous cannot get path \"/\"'), which is an exposure worth\n    reporting to AcreTrader. api.acretrader.com is a distinct address (34.111.83.6)\n    and is a real service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acretrader/refs/heads/main/security/acretrader-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Farmland
- Investing
- Alternative Investments
- Real Estate
- Fintech
- Agriculture
- Marketplace
- Farmland Investing
- Accredited Investors
- Private Placements
- AgTech
---
