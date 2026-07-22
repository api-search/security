---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datagrail.io
  spf: true
hosts:
- cert_expires: Sep 16 01:47:17 2026 GMT
  host: www.datagrail.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datagrail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataGrail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataGrail
provider_slug: datagrail
slug: datagrail-domain-security
source_filename: datagrail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datagrail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:47:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datagrail.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datagrail/refs/heads/main/security/datagrail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Privacy
- Data Privacy
- Privacy Operations
- Compliance
- GDPR
- CCPA
- Data Subject Requests
- DSR
- Consent Management
- Cookie Compliance
- Risk Management
- Privacy Impact Assessments
- DPIA
- AI Risk
- Data Mapping
- Data Discovery
- SaaS
- Enterprise
---
