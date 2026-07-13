---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uscourts.gov
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.cafc.uscourts.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: pacer.uscourts.gov
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Court Of Appeals For The Federal Circuit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Court of Appeals for the Federal Circuit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: US Court of Appeals for the Federal Circuit
provider_slug: us-court-of-appeals-for-the-federal-circuit
slug: us-court-of-appeals-for-the-federal-circuit-domain-security
source_filename: us-court-of-appeals-for-the-federal-circuit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cafc.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n- host: pacer.uscourts.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: uscourts.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-court-of-appeals-for-the-federal-circuit/refs/heads/main/security/us-court-of-appeals-for-the-federal-circuit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federal Government
- Legal
- Patent Law
- Federal Courts
- Appellate Courts
---
