---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fca.gov
  spf: true
hosts:
- cert_expires: '2026-11-01'
  host: www.fca.gov
  hsts: null
  https: true
  note: The public www site is the ONLY probed FCA host with no Strict-Transport-Security header; every application host below sets max-age=31536000; preload.
  tls_version: TLSv1.3
- cert_expires: '2027-01-08'
  cert_issuer: Entrust OV TLS Issuing RSA CA 2
  host: wgis.fca.gov
  hsts: max-age=31536000; preload
  https: true
  role: ArcGIS REST API host (the record's only machine-readable API surface)
  tls_version: TLSv1.2
- cert_expires: '2027-02-12'
  cert_issuer: Entrust OV TLS Issuing RSA CA 2
  host: apps.fca.gov
  hsts: max-age=31536000; preload
  https: true
  role: FCS Public Directory + Locator web applications
  tls_version: TLSv1.2
- cert_expires: '2026-12-11'
  cert_issuer: Entrust OV TLS Issuing RSA CA 2
  host: reports.fca.gov
  hsts: max-age=31536000; preload
  https: true
  role: Consolidated Reporting System (CRS) call-report web application
  tls_version: TLSv1.2
- host: ww4.fca.gov
  https: null
  note: DNS resolves to 4.79.206.89 but TCP connect to 443 and 80 times out from the public internet. Could not be probed. This is the host behind FCA's own "FCS Data Portal" link.
hosts_probed: 5
kind: domain-security
layout: security
method: probed
name: Farm Credit Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farm Credit Administration, probed live across 5 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Farm Credit Administration
provider_slug: farm-credit-administration
slug: farm-credit-administration-domain-security
source_filename: farm-credit-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts, the ArcGIS REST API host, and every host named in\n  FCA's own Vulnerability Disclosure Policy scope section\nhosts:\n  - host: www.fca.gov\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: '2026-11-01'\n    hsts: null\n    note: >-\n      The public www site is the ONLY probed FCA host with no Strict-Transport-Security header;\n      every application host below sets max-age=31536000; preload.\n  - host: wgis.fca.gov\n    https: true\n    tls_version: TLSv1.2\n    cert_issuer: Entrust OV TLS Issuing RSA CA 2\n    cert_expires: '2027-01-08'\n    hsts: max-age=31536000; preload\n    role: ArcGIS REST API host (the record's only machine-readable API surface)\n  - host: apps.fca.gov\n    https: true\n    tls_version: TLSv1.2\n    cert_issuer: Entrust OV TLS Issuing RSA CA 2\n    cert_expires: '2027-02-12'\n    hsts: max-age=31536000; preload\n    role: FCS Public Directory\
  \ + Locator web applications\n  - host: reports.fca.gov\n    https: true\n    tls_version: TLSv1.2\n    cert_issuer: Entrust OV TLS Issuing RSA CA 2\n    cert_expires: '2026-12-11'\n    hsts: max-age=31536000; preload\n    role: Consolidated Reporting System (CRS) call-report web application\n  - host: ww4.fca.gov\n    https: null\n    note: >-\n      DNS resolves to 4.79.206.89 but TCP connect to 443 and 80 times out from the public internet.\n      Could not be probed. This is the host behind FCA's own \"FCS Data Portal\" link.\ndomains:\n  - domain: fca.gov\n    dnssec: true\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/farm-credit-administration/refs/heads/main/security/farm-credit-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agriculture
- Farms
- Federal-Government
- Finance
- Regulations
- Geospatial
- Open-Data
- Banking
- Lending
- Government
---
