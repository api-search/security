---
description: AcreTrader publishes no public API and declares no baseURL/OpenAPI servers, so the primary corporate web host acretrader.com was probed directly. Absence of a record (CAA, DNSSEC, HSTS) is valid, expected data for a marketing/investment site, not a gap in an API surface.
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
  spf: true
  spf_record: v=spf1 mx include:_spf.google.com ip4:152.70.150.118 ip4:129.213.11.79 include:spf.protection.outlook.com include:sendgrid.net -all
hosts:
- cert_expires: Sep  7 06:28:46 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  csp: false
  host: acretrader.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Served from Google Cloud (UploadServer signature). www.acretrader.com redirects to the apex host.
  server: UploadServer
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acretrader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acretrader, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acretrader
provider_slug: acretrader
slug: acretrader-domain-security
source_filename: acretrader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of acretrader.com (no API baseURL/servers hosts in apis.yml)\ndescription: >-\n  AcreTrader publishes no public API and declares no baseURL/OpenAPI servers, so\n  the primary corporate web host acretrader.com was probed directly. Absence of a\n  record (CAA, DNSSEC, HSTS) is valid, expected data for a marketing/investment\n  site, not a gap in an API surface.\nhosts:\n  - host: acretrader.com\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: Google Trust Services (WR3)\n    cert_expires: Sep  7 06:28:46 2026 GMT\n    hsts: false\n    hsts_max_age: null\n    csp: false\n    server: UploadServer\n    note: >-\n      Served from Google Cloud (UploadServer signature). www.acretrader.com\n      redirects to the apex host.\ndomains:\n  - domain: acretrader.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: >-\n      v=spf1 mx include:_spf.google.com ip4:152.70.150.118 ip4:129.213.11.79\n\
  \      include:spf.protection.outlook.com include:sendgrid.net -all\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_rua: mailto:admin@acretrader.com\n    nameservers:\n      - ns-cloud-b1.googledomains.com\n      - ns-cloud-b2.googledomains.com\n      - ns-cloud-b3.googledomains.com\n      - ns-cloud-b4.googledomains.com\n"
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
---
