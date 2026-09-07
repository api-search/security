---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:admin@hud.gov"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hud.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: huduser.gov
  spf: true
hosts:
- cert_expires: Nov 24 09:14:15 2026 GMT
  host: www.hud.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 00:37:34 2027 GMT
  host: www.huduser.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: hudgis-hud.opendata.arcgis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Department Of Housing And Urban Development Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Housing and Urban Development, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Housing and Urban Development
provider_slug: department-of-housing-and-urban-development
slug: department-of-housing-and-urban-development-domain-security
source_filename: department-of-housing-and-urban-development-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hud.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 09:14:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.huduser.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 00:37:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hudgis-hud.opendata.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hud.gov\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:admin@hud.gov\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: huduser.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-housing-and-urban-development/refs/heads/main/security/department-of-housing-and-urban-development-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Affordable Housing
- Fair Market Rents
- Federal-Government
- FHA
- GIS
- Housing
- HUD
- Income Limits
- Mortgage
- Open Data
---
