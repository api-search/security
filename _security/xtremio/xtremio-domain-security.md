---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9"
  - 0 iodef "mailto:pkiadmin@dell.com"
  dmarc: true
  dmarc_policy: reject
  dmarc_record: v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com; ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com;
  dnssec: false
  domain: xtremio.com
  mx: []
  spf: true
  spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all
hosts:
- host: xtremio.com
  hsts: false
  https: false
  https_note: port 443 accepts TCP but the TLS handshake fails (alert internal error, no certificate served); HTTP (port 80) serves a Safenames parked placeholder page
- host: www.xtremio.com
  hsts: false
  https: false
  https_note: same parked infrastructure as apex (A 217.19.248.132)
kind: domain-security
layout: security
method: probed
name: Xtremio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XtremIO, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: XtremIO
provider_slug: xtremio
slug: xtremio-domain-security
source_filename: xtremio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS handshake probes of xtremio.com (manual probe pass; apis.yml has no\n  Website/baseURL for the script to walk — company was acquired and the domain is parked)\nnote: XtremIO was acquired by EMC in May 2012; the xtremio.com domain is retained under\n  Dell brand protection (Safenames registrar parked page). DNS mail-security posture is\n  actively managed (Proofpoint SPF/DMARC, Dell PKI CAA) but no HTTPS website is served.\nhosts:\n  - host: xtremio.com\n    https: false\n    https_note: port 443 accepts TCP but the TLS handshake fails (alert internal error,\n      no certificate served); HTTP (port 80) serves a Safenames parked placeholder page\n    hsts: false\n  - host: www.xtremio.com\n    https: false\n    https_note: same parked infrastructure as apex (A 217.19.248.132)\n    hsts: false\ndomains:\n  - domain: xtremio.com\n    dnssec: false\n    caa:\n      - 0 issue \"digicert.com; account=b34fd286db03ccad020f0a75010dd75544eaf2b967195b4becb6460c924d35c9\"\
  \n      - 0 iodef \"mailto:pkiadmin@dell.com\"\n    spf: true\n    spf_record: v=spf1 include:%{ir}.%{v}.%{d}.spf.has.pphosted.com -all\n    dmarc: true\n    dmarc_policy: reject\n    dmarc_record: v=DMARC1; p=reject; fo=1; rua=mailto:dmarc_rua@emaildefense.proofpoint.com;\n      ruf=mailto:dmarc_ruf@emaildefense.proofpoint.com;\n    mx: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xtremio/refs/heads/main/security/xtremio-domain-security.yml
summary_line: DMARC
tags:
- Company
- Storage
- Flash Storage
- Enterprise Storage
- Data Center
- Acquired
---
