---
description: ''
domains:
- caa:
  - 0 issuewild "quovadisglobal.com"
  - 0 iodef "mailto:soc@kadaster.nl"
  - 0 issue "certSIGN.ro"
  - 0 issue "digicert.com"
  - 0 issue "kpn.com"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kadaster.nl
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.kadaster.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kadaster International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadaster International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kadaster International
provider_slug: kadaster-international
slug: kadaster-international-domain-security
source_filename: kadaster-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kadaster.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kadaster.nl\n  dnssec: true\n  caa:\n  - 0 issuewild \"quovadisglobal.com\"\n  - 0 iodef \"mailto:soc@kadaster.nl\"\n  - 0 issue \"certSIGN.ro\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"kpn.com\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kadaster-international/security/kadaster-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Land Registry
- Geospatial
- Real Estate
- Government
- Netherlands
---
