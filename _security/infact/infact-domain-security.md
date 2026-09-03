---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: infact.solutions
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hpzone.nl
  spf: false
hosts:
- cert_expires: Oct 25 12:29:26 2026 GMT
  host: infact.solutions
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.hpzone.nl
  https: false
kind: domain-security
layout: security
method: probed
name: Infact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InFact, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InFact
provider_slug: infact
slug: infact-domain-security
source_filename: infact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: infact.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 12:29:26 2026 GMT\n  hsts: false\n- host: api.hpzone.nl\n  https: false\ndomains:\n- domain: infact.solutions\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hpzone.nl\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\nnotes:\n- api.hpzone.nl shows https:false because the probe tests port 443. The HPZone API is served on port 8899,\n  which our network could not reach either (TCP connect timeout on all three A records, single bounded\n  attempt). No conclusion should be drawn about the API host's TLS posture from this row.\n- infact.solutions serves TLS 1.3 but sets no HSTS header. The site sits behind a SiteGround JavaScript\n  bot challenge (HTTP 202 on every path), which is what the HEAD probe reached.\n- DMARC is published at\
  \ p=none — monitoring only, no enforcement — on a domain belonging to a supplier\n  of national public-health case-management systems.\n- Neither infact.solutions nor hpzone.nl publishes DNSSEC or a CAA record. hpzone.nl publishes no SPF\n  and no DMARC at all; its root is a parked GoDaddy lander, while the operational API lives at api.hpzone.nl:8899.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infact/refs/heads/main/security/infact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Public Health
- Healthcare
- Epidemiology
- Disease Surveillance
- Outbreak Management
- Contact Tracing
- Electronic Health Records
- openEHR
- GraphQL
- Government
---
