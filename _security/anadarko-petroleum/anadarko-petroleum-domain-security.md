---
description: ''
domains:
- caa:
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: false
  domain: anadarko.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oxy.com
  spf: true
hosts:
- host: www.anadarko.com
  https: false
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.oxy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anadarko Petroleum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anadarko Petroleum, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Anadarko Petroleum
provider_slug: anadarko-petroleum
slug: anadarko-petroleum-domain-security
source_filename: anadarko-petroleum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anadarko.com\n  https: false\n- host: www.oxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anadarko.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: false\n- domain: oxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anadarko-petroleum/refs/heads/main/security/anadarko-petroleum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Deepwater
- Energy
- Natural Gas
- Oil And Gas
- Petroleum
- Upstream
- Fortune 500
---
