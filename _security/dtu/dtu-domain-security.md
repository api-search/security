---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:ait-dmarcaggregate@dtu.dk; ruf=mailto:ait-dmarcreport@dtu.dk; pct=100; fo=1
  dnssec: false
  domain: dtu.dk
  spf: true
hosts:
- cert_expires: Nov 18 09:00:56 2026 GMT
  host: www.dtu.dk
  hsts: false
  https: true
  tls_version: TLSv1.3
  x-operator: institution
- cert_expires: Feb 12 08:30:58 2027 GMT
  host: sts.ait.dtu.dk
  hsts: false
  https: true
  note: DTU security token service (AD FS); serves signed SAML metadata and OIDC discovery.
  x-operator: institution
- cert_expires: Oct 13 04:26:27 2026 GMT
  host: findit.dtu.dk
  hsts: false
  https: true
  note: DTU Findit library discovery (Blacklight).
  x-operator: institution
- cert_expires: Nov 22 07:00:17 2026 GMT
  host: wps.globalwindatlas.info
  hsts: false
  https: true
  note: Global Wind Atlas OGC WPS; ows:ServiceProvider is DTU Wind Energy, contact neda@dtu.dk.
  x-operator: institution
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: data.dtu.dk
  hsts: false
  https: true
  note: DTU Data — Figshare tenant host. Behind an AWS WAF challenge for non-browser clients.
  x-operator: tenant
kind: domain-security
layout: security
method: probed
name: Dtu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technical University of Denmark, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Technical University of Denmark
provider_slug: dtu
slug: dtu-domain-security
source_filename: dtu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live DNS/TLS/HTTP probes of the hosts named in apis.yml. Vendor hosts previously carried here\n  (api.figshare.com, figshare.com) were removed with the vendor contracts they came from — their\n  posture is Figshare's, not DTU's, and crediting it to DTU is the misattribution this repo was\n  corrected for.\nhosts:\n- host: www.dtu.dk\n  x-operator: institution\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 09:00:56 2026 GMT\n  hsts: false\n- host: sts.ait.dtu.dk\n  x-operator: institution\n  note: DTU security token service (AD FS); serves signed SAML metadata and OIDC discovery.\n  https: true\n  cert_expires: Feb 12 08:30:58 2027 GMT\n  hsts: false\n- host: findit.dtu.dk\n  x-operator: institution\n  note: DTU Findit library discovery (Blacklight).\n  https: true\n  cert_expires: Oct 13 04:26:27 2026 GMT\n  hsts: false\n- host: wps.globalwindatlas.info\n  x-operator: institution\n  note: Global Wind Atlas\
  \ OGC WPS; ows:ServiceProvider is DTU Wind Energy, contact neda@dtu.dk.\n  https: true\n  cert_expires: Nov 22 07:00:17 2026 GMT\n  hsts: false\n- host: data.dtu.dk\n  x-operator: tenant\n  note: DTU Data — Figshare tenant host. Behind an AWS WAF challenge for non-browser clients.\n  https: true\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dtu.dk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_record: >-\n    v=DMARC1; p=quarantine; rua=mailto:ait-dmarcaggregate@dtu.dk;\n    ruf=mailto:ait-dmarcreport@dtu.dk; pct=100; fo=1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dtu/refs/heads/main/security/dtu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Technical University
- Denmark
- Europe
- Identity Federation
- Research Data
- Library
- Course Catalog
- Wind Energy
---
