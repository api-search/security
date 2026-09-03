---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ameresco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assetplanner.com
  spf: true
hosts:
- cert_expires: Oct 17 20:32:30 2026 GMT
  host: www.ameresco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: assetplanner.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ameresco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ameresco, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ameresco
provider_slug: ameresco
slug: ameresco-domain-security
source_filename: ameresco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ameresco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 20:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: assetplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ameresco.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: assetplanner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: 'assetplanner.com is added by hand: it is the host serving Ameresco''s own AssetPlanner platform\n  (login footer ''Ameresco 2026'', links to ameresco.com/asset-planning-software-solutions/,\
  \ cert CN=*.assetplanner.com)\n  but is not named by any apis.yml baseURL, so the automated host collector does not reach it. Probed\n  2026-09-02 by the same method as the rest of this file.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ameresco/refs/heads/main/security/ameresco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy Efficiency
- Clean Energy
- Energy Management
- Asset Management
- Facilities
- Sustainability
- Infrastructure
- Services
---
