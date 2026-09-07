---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: seaboardcorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: seaboardmarine.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: seaboardfoods.com
  note: DMARC published via a CNAME delegation to Proofpoint (dmarc.has.pphosted.com).
  spf: true
- domain: seaboard.com
  note: NXDOMAIN as of 2026-09-04. Not a Seaboard Corporation domain; the catalog Website pointer that named it has been corrected to seaboardcorp.com.
  resolves: false
hosts:
- cert_expires: Nov  3 06:36:25 2026 GMT
  host: www.seaboardcorp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.seaboardmarine.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: myseaboard.seaboardmarine.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  note: MySeaboard customer portal; every path probed returns 302 to the login.
  tls_version: TLSv1.2
- cert_expires: Nov 17 04:07:23 2026 GMT
  host: www.seaboardfoods.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Seaboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seaboard, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Seaboard
provider_slug: seaboard
slug: seaboard-domain-security
source_filename: seaboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + subsidiary operating hosts (seaboardcorp.com by probe-domain-security.py;\n  seaboardmarine.com, myseaboard.seaboardmarine.com and seaboardfoods.com probed by hand in the same pass)\nhosts:\n- host: www.seaboardcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 06:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.seaboardmarine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: myseaboard.seaboardmarine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n  note: MySeaboard customer portal; every path probed returns 302 to the login.\n- host: www.seaboardfoods.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 04:07:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\ndomains:\n- domain:\
  \ seaboardcorp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: seaboardmarine.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: seaboardfoods.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: DMARC published via a CNAME delegation to Proofpoint (dmarc.has.pphosted.com).\n- domain: seaboard.com\n  resolves: false\n  note: NXDOMAIN as of 2026-09-04. Not a Seaboard Corporation domain; the catalog Website pointer that named it\n    has been corrected to seaboardcorp.com.\nnote: Seaboard Corporation operates its subsidiaries on separate registrable domains. The corporate domain is seaboardcorp.com;\n  www.seaboard.com (previously carried as the Website pointer) does not resolve at all. Subsidiary hosts are probed\n  here because they are where any integration surface would live.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seaboard/refs/heads/main/security/seaboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fortune 500
- Agribusiness
- Ocean Transportation
- Container Shipping
- Pork Production
- Commodity Trading
- Grain Milling
- Power Generation
- Logistics
- EDI
---
