---
api_specs:
- filename: epignosis-talentlms-efront-talentcards-efront-openapi-original.json
  format: json
  label: eFront API
  slug: efront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epignosis-talentlms-efront-talentcards/refs/heads/main/openapi/epignosis-talentlms-efront-talentcards-efront-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epignosishq.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "entrust.net"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: talentlms.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.epignosishq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: www.talentlms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: samples.talentlms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epignosis Talentlms Efront Talentcards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epignosis (TalentLMS, eFront, TalentCards), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epignosis (TalentLMS, eFront, TalentCards)
provider_slug: epignosis-talentlms-efront-talentcards
slug: epignosis-talentlms-efront-talentcards-domain-security
source_filename: epignosis-talentlms-efront-talentcards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epignosishq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\n- host: www.talentlms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: samples.talentlms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epignosishq.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: talentlms.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"entrust.net\"\n  -\
  \ 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epignosis-talentlms-efront-talentcards/refs/heads/main/security/epignosis-talentlms-efront-talentcards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Learning Management System
- LMS
- Training
- eLearning
- Microlearning
- Corporate Training
- SaaS
---
