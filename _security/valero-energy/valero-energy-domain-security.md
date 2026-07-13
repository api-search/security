---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valero.com
  spf: true
- caa:
  - 0 issue "entrust.net"
  - 0 iodef "mailto:CAIssues@sec.gov"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sec.gov
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.valero.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.sec.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:46:07 2026 GMT
  host: investorvalero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valero Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valero Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Valero Energy
provider_slug: valero-energy
slug: valero-energy-domain-security
source_filename: valero-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.valero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.sec.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: investorvalero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:46:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: valero.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sec.gov\n  dnssec: true\n  caa:\n  - 0 issue \"entrust.net\"\n  - 0 iodef \"mailto:CAIssues@sec.gov\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valero-energy/refs/heads/main/security/valero-energy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Petroleum
- Refining
- Renewable Fuels
- Fortune 100
- Ethanol
- Renewable Diesel
---
