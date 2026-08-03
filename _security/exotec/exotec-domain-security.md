---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exotec.com
  spf: true
hosts:
- cert_expires: Oct 18 12:30:12 2026 GMT
  host: www.exotec.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exotec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exotec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exotec
provider_slug: exotec
slug: exotec-domain-security
source_filename: exotec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exotec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 12:30:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: exotec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nobservations:\n- kind: dangling-cname\n  host: api.exotec.com\n  record: CNAME dc50zvit13.execute-api.eu-west-3.amazonaws.com.\n  target_resolves: false\n  target_status: NXDOMAIN\n  resolvers_checked: [8.8.8.8, 1.1.1.1, system]\n  fetched: '2026-07-31'\n  note: >-\n    api.exotec.com still publishes a CNAME to an AWS API Gateway regional custom domain\n    in eu-west-3 whose target no longer resolves (NXDOMAIN). The API host is therefore\n    unreachable, and an unclaimed API Gateway custom-domain CNAME is the classic\n    subdomain-takeover exposure class. Recorded as observed DNS data only.\n- kind: no-caa\n\
  \  domain: exotec.com\n  note: No CAA records published, so certificate issuance is not restricted to named CAs.\n- kind: no-dnssec\n  domain: exotec.com\n  note: DNSSEC is not enabled on exotec.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exotec/refs/heads/main/security/exotec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Warehouse Automation
- Robotics
- Logistics
- Supply Chain
- Fulfillment
- Warehouse Execution System
- Warehouse Management
- Industrial Automation
- Manufacturing
---
