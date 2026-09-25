---
api_specs:
- filename: 2sAYQZJYMC
  format: yaml
  label: GreyMatter API
  slug: greymatter-api
  spec_type: Postman
  url: https://apidocs.myreliaquest.com/api/collections/39440280/2sAYQZJYMC?segregateAuth=true&versionTag=latest
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reliaquest.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: myreliaquest.com
  spf: true
hosts:
- cert_expires: Nov  3 20:53:47 2026 GMT
  host: reliaquest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 10:05:57 2026 GMT
  host: apidocs.myreliaquest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: greymatter.myreliaquest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Reliaquest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReliaQuest, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ReliaQuest
provider_slug: reliaquest
slug: reliaquest-domain-security
source_filename: reliaquest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reliaquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 20:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.myreliaquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 10:05:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: greymatter.myreliaquest.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reliaquest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: myreliaquest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliaquest/refs/heads/main/security/reliaquest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Security Operations
- Threat Detection
- Incident Response
- Threat Intelligence
- Digital Risk Protection
- AI Agents
- GraphQL
---
