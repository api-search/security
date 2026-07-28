---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: southerncompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; aspf=s; pct=100; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com
  dnssec: false
  domain: southernco.com
  spf: true
  spf_record: v=spf1 redirect=spf-enabled.southernco.com
hosts:
- cert_expires: Oct 15 01:33:25 2026 GMT
  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2
  cert_subject: CN=imperva.com
  host: www.southerncompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 01:33:25 2026 GMT
  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2
  cert_subject: CN=imperva.com
  host: api.southernco.com
  hsts: true
  hsts_max_age: 86400
  https: true
  note: Apigee Edge gateway; every path returns the ApplicationNotFound fault (see review.yml)
  tls_version: TLSv1.3
- cert_expires: Oct 15 01:33:25 2026 GMT
  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2
  cert_subject: CN=imperva.com
  host: customerservice2.southerncompany.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 01:33:25 2026 GMT
  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2
  cert_subject: CN=imperva.com
  host: webauth.southernco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 01:33:25 2026 GMT
  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2
  cert_subject: CN=imperva.com
  host: www.georgiapower.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Southern Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Southern Company, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Southern Company
provider_slug: southern-company
slug: southern-company-domain-security
source_filename: southern-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts, the Apigee gateway host and the\n  customer-portal hosts named in review.yml\nnote: >-\n  Every Southern Company host probed terminates TLS on the Imperva edge and presents the\n  same shared GlobalSign DV certificate (subject CN=imperva.com, expires Oct 15 2026) on an\n  anonymous handshake — there is no customer-named certificate on the default response.\n  HSTS is present everywhere but the max-age is inconsistent across the estate (86,400s on\n  the API gateway vs 31,536,000s on the corporate site). Neither registrable domain signs\n  with DNSSEC or publishes a CAA record; both publish SPF and a DMARC policy of `reject`.\nhosts:\n- host: www.southerncompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=imperva.com\n  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2\n  cert_expires: Oct 15 01:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.southernco.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=imperva.com\n  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2\n  cert_expires: Oct 15 01:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n  note: Apigee Edge gateway; every path returns the ApplicationNotFound fault (see review.yml)\n- host: customerservice2.southerncompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=imperva.com\n  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2\n  cert_expires: Oct 15 01:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: webauth.southernco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=imperva.com\n  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2\n  cert_expires: Oct 15 01:33:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.georgiapower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_subject: CN=imperva.com\n  cert_issuer: GlobalSign Atlas R46 DV TLS CA 2026 Q2\n  cert_expires: Oct 15 01:33:25 2026 GMT\n  hsts:\
  \ true\n  hsts_max_age: 31536000\ndomains:\n- domain: southerncompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: southernco.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 redirect=spf-enabled.southernco.com\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_record: 'v=DMARC1; p=reject; aspf=s; pct=100; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com;\n    ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/southern-company/refs/heads/main/security/southern-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Grid
- Smart Metering
- Nuclear
- Energy Markets
- Renewables
---
